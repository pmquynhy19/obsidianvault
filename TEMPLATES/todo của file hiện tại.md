#### Todo còn
```dataview
task
where !completed and file.name = this.file.name
```
##### Quote tổng hợp
```dataviewjs
let file = dv.current().file;

app.vault.read(app.vault.getAbstractFileByPath(file.path)).then(content => {
  const lines = content.split("\n");
  for (let line of lines) {
    if (line.trim().startsWith(">")) {
      dv.paragraph(line);
    }
  }
});
```
#flashcard

# Heading 1
- [x] abc
> quote nè