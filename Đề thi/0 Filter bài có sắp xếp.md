```dataviewjs
dv.paragraph("📚 Tổng hợp câu sai — gom theo từng bài:");

let grouped = {};

for (let page of dv.pages()) {
  for (let block of page.file.lists || []) {
    let line = block.text.trim();
    if (!line.startsWith("bài ")) continue;

    let parts = line.split(" ");
    if (parts.length < 3) continue;

    let tenBai = parts[1];
    let kieuKT = parts[2];
    let cleanedText = line.replace(/!\[\[.*?\]\]/g, "").trim();

    if (!grouped[tenBai]) grouped[tenBai] = {};
    if (!grouped[tenBai][kieuKT]) grouped[tenBai][kieuKT] = [];

    grouped[tenBai][kieuKT].push({
      text: cleanedText,
      fileName: page.file.name,
      path: page.file.path
    });
  }
}

for (let tenBai of Object.keys(grouped).sort()) {
  dv.header(1, "📘 Bài: " + tenBai.toUpperCase());

  for (let kieuKT of Object.keys(grouped[tenBai]).sort()) {
    dv.header(3, "🔹 " + kieuKT.toUpperCase());

    for (let item of grouped[tenBai][kieuKT]) {
      dv.el("div", `➤ <a href="${item.path}">${item.fileName}</a>: ${item.text}`);
    }

    dv.el("br", "");
  }
}
