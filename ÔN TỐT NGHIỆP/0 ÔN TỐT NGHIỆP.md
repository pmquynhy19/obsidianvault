Plan: [[CHIA-LỊCH-HỌC-TỐT-NGHIỆP 1.pdf]]
Protocol: [[tot nghiep protocol]]

---
```dataviewjs
dv.table(["Bài", "Ngày học", "Ghi chú"],
  dv.pages('"ÔN TỐT NGHIỆP"')
    .where(p => !p.file.name.startsWith("0"))  // loại file bắt đầu bằng "0"
    .sort(p => p.created, 'desc')
    .map(p => [p.file.link, p.created, p.note])
);
```
---

|         |             |                                        |            |               |                                 |           |         |
| ------- | ----------- | -------------------------------------- | ---------- | ------------- | ------------------------------- | --------- | ------- |
|         | 7h30 – 8h30 | 8h30 – 10h                             | 10h – 12h  | 13h30 – 15h30 | 15h30 – 17h                     | 19h – 20h | TIẾN ĐỘ |
|         | 1 buổi lớn  | <font color="#ff0000">làm đề có đáp án | 1 buổi lớn | 4 buổi nhỏ    | làm đề                          |           |         |
| N1 5/11 |             |                                        |            |               | 14 câu<br>[[0 NHIỄM NGƯỜI LỚN]] |           |         |
|         |             |                                        |            |               |                                 |           |         |
ĐỀ TN

Y16
* [[TN Nội Y16 1]]
	* file1 [[Đề tốt nghiệp hệ Nội - Y16 (Lần 1) 1.pdf]]
* [[TN Nội Y16 2]]
	* file2: [[Tốt-nghiệp-lần-2-hệ-Nội-Y16.pdf]]
* [[TN Nội Y15]]
	* file: [[Đề tốt nghiệp hệ Nội - Y15 (Lần 1).pdf]] 