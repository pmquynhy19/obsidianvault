```dataviewjs
dv.paragraph("📚 Các câu sai về cận lâm sàng:");

for (let page of dv.pages()) {
  for (let block of page.file.lists || []) {
    if (block.text.includes("#canonlai")) {
      dv.paragraph("- [[" + page.file.path + "|" + page.file.name + "]]: " + block.text);
    }
  }
}

