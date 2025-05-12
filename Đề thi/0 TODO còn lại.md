```dataviewjs
dv.taskList(
  dv.pages()
    .where(p => !p.file.path.includes("Đề thi") && !p.file.path.includes("TODO"))
    .file.tasks
    .where(t => !t.completed),
  true
);

for (let page of dv.pages()) {
  let tasks = page.file.tasks.where(t => !t.completed);
  for (let task of tasks) {
    if (!page.file.path.includes("Đề thi") && !page.file.path.includes("todo khi đánh đề")) {
      dv.paragraph("> 🗂 Nguồn: [[" + page.file.name + "]]");
    }
  }
}

