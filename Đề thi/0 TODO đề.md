## ❌ Các câu sai chưa ôn lại (unchecked todo)

```dataviewjs
let pages = dv.pages('"Đề thi"')
  .where(p => p.file.tasks.some(t => !t.completed));

for (let page of pages) {
  let tasks = page.file.tasks.where(t => !t.completed);
  dv.taskList(tasks, true);
  dv.paragraph("> 🗂 Nguồn: [[" + page.file.name + "]]");
}
