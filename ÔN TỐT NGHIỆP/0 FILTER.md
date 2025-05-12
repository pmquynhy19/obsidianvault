```dataviewjs
const FOLDER = "ÔN TỐT NGHIỆP";

// Danh sách từ khóa cần lọc
const keywords = {
  "🔁 Xem mỗi ngày (thuongxuyen)": "#thuongxuyen",
  "🧠 Mẹo ghi nhớ (mnemonic)": "#meo",
  "❌ Câu từng sai (cauhoitungsai)": "#cauhoitungsai",
  "🎯 Trọng tâm đề thi (trongtam)": "#trongtam",
  "📌 Thầy cô nhấn mạnh (thi)": "#thi",
  "🧠 Cần học lại kỹ (thuoclong)": "#thuoclong"
};

// Lặp từng loại từ khóa để lọc
for (let [label, keyword] of Object.entries(keywords)) {
  dv.header(2, label);

  for (let page of dv.pages(`"${FOLDER}"`)) {
    for (let block of page.file.lists || []) {
      if (block.text.toLowerCase().includes(keyword.toLowerCase())) {
        dv.paragraph("- [[" + page.file.name + "]]: " + block.text);
      }
    }
  }
}
