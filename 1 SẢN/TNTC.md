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
# Định tuổi thai và các vấn đề liên quan

## Kinh chót

- [x] **Các trường hợp không dùng** ngày kinh cuối để tính tuổi thai
	- Người quên ngày kinh hoặc chỉ cho thông tin mơ hồ
	- Người đã từng có chu kì kinh dài từ ≥ 31 ngày
	- Người có các chu kì kinh không đều (chênh lệch ≥ 7 ngày - uptodate)
	- Lần “hành kinh” cuối có tính chất “khác lạ”
	- Người đã từng có các chu kì không phóng noãn
	- Người có dùng hormones trong chu kì có thai (steroid ngoại sinh, Gn ngoại sinh)

- [x] ĐK dùng + ? #tìm
	**Chu kỳ kinh tin cậy là 26-30 ngày.**

> Khuyến cáo tính tuổi thai bằng siêu âm khi thai được 10 tuần tuổi theo ước tính.

> Trong các trường hợp được yêu cầu, hoặc xuất hiện các biến cố (xuất huyết, hết nghén) thì sẽ có chỉ định siêu âm sớm hơn – 8 tuần.

IVF: tuổi thai được xác định, không được thay thế bằng bất kì thông tin nào khác. Nhớ lùi 14 ngày.

## Siêu âm để định tuổi thai

Siêu âm định tuổi thai có thể thực hiện khi CRL từ 10-84, tuy nhiên chỉ thực sự tin cậy khi CRL từ 30-84 (thai 10-13+6 tuần tuổi), khi đó sai số tuổi thai là ± 5 ngày.

[https://fetalmedicine.org/research/pregnancyDating](https://fetalmedicine.org/research/pregnancyDating)
> Trong trường hợp CRL < 30, có thể tạm tính tuổi thai là ==CRL + 42==
<!--SR:!2025-05-08,4,270-->

- [ ] **dấu bằng ở đâu?** Khi có kết quả tuổi thai qua siêu âm (CRL tiêu chuẩn), nếu sai số < 7 ngày so với “ngày kinh cuối” thì tuổi thai nên tính theo ngày kinh cuối, nếu > 7 ngày thì nên tính theo siêu âm

Trường hợp siêu âm khi thai ≤ 9 tuần tuổi, sai số < 5 ngày thì tuổi thai sẽ tính theo “ngày kinh cuối”

> Trường hợp siêu âm ra nhiều kết quả CRL, ưu tiên chọn CRL thực hiện sớm nhất trong khoảng ==30 - 84== mm.
<!--SR:!2025-05-09,3,252-->

> Từ tuần 11, có thể định tuổi thai bằng BPD (đường kính lưỡng đỉnh) hoặc HC (vòng đầu). Nhưng chỉ dùng khi thai phụ ko có siêu âm nào có CRL 10-84, và hiện tại đã >84.

ISUOG nhận định HC ==tốt== hơn BPD trong lĩnh vực định tuổi thai. FMF tính tuổi thai bằng HC khi HC từ 100-280 mm. (13 tuần 3/7 đến 28 tuần 5/7)
<!--SR:!2025-05-09,3,252-->

[https://fetalmedicine.org/research/pregnancyDating](https://fetalmedicine.org/research/pregnancyDating)

BPD là 17mm khi thai 11 tuần tròn, từ tuần 13 đến 26 tăng 3mm/tuần.

> Tuổi thai = (BPD – 17)/3 + ==11== (tuần)
<!--SR:!2025-05-09,3,252-->

> Công thức Naegele: Ngày dự sanh = ==(ngày +7) / (tháng – 3) / (năm +1)==
(cộng 9 tháng 7 ngày)
<!--SR:!2025-05-09,3,252-->

Xác định tuổi thai càng trễ -> càng không chính xác. Ở TCN II lệch từ 7-12 ngày. Ở TCN III lệch đến 18-35 ngày.

> Lưu ý: không dùng MSD (đường kính trung bình túi thai) và Yolk-sac để định tuổi thai._

# Thai nghén thất bại sớm (Early pregnancy loss)


Thuật ngữ: sẩy thai, tiếng anh là pregnancy loss/miscarriage/spontaneous abortion, là khái niệm chỉ thai chết trong lòng tử cung trước 20 tuần tuổi thai. EPL, sẩy thai trong TCN1 là dạng thường gặp nhất. [2]

80% sẩy thai xảy ra trong TCN1, 50% EPL là do lệch bội.

EPL chiếm 30% tổng số thai kỳ theo ước tính, EPL được chẩn đoán xác định chiếm 10% tổng số thai kỳ 🡪 rất thường gặp.

Hồi trước ngta nghĩ Aspirin giúp giảm tỉ lệ EPL do thrombophilias là 1 nguyên nhân gây sẩy thai. Nhưng ACOG thấy việc sử dụng thuốc chống đông, aspirin không làm giảm nguy cơ EPL ở phụ nữ mắc thrombophilias, trừ trường hợp mắc hội chứng anti-phospholipid. [6]

Các khái niệm:

- Có thai sinh hóa: khi test B-hCG (+) trong máu/nước tiểu
- Có thai lâm sàng: phát hiện có thai qua hình ảnh học
- ==Trứng trống== (blighted ovum, ngày nay là anembryonic pregnancy): túi thai không phôi
- EPL: có thai LÂM SÀNG, nhưng không có tim thai
<!--SR:!2025-05-09,3,252-->

> Định nghĩa sẩy thai: thai kì sụp đổ tự phát trước khi thai nhi có khả năng sinh sống (24 tuần)

> EPL có thể phân ra:
	- Thai chết lưu (missed miscarriage): thai chết lưu mà mình không biết (bỏ lỡ)
	- Dọa sẩy thai lưu (threatened miscarriage): rất nghi ngờ thai lưu, nhưng chưa chẩn đoán
	- Sẩy thai khó tránh (inevitable miscarriage): ==đang sẩy==
	- Sẩy thai không trọn (incomplete miscarriage): sẩy gần xong
	- Sẩy thai trọn (complete miscarriage): đã sẩy xong
<!--SR:!2025-05-09,3,252-->

Tuy nhiên những thuật ngữ này quá khó để phân định và chưa đầy đủ thông tin, nên chỉ còn là lịch sử để lại. Hiện nay người ta ưu tiên ghi rõ ra những gi nhìn thấy được. VD: thay vì sẩy thai không trọn, giờ ghi là “túi thai trống dai dẳng mặc dù được chẩn đoán ban đầu là không thể sống được từ … tuần trước”.

## Lâm sàng

Chảy máu và đau bụng chưa biến chứng: là triệu chứng thường gặp nhất, “chưa biến chứng” ngụ ý là BN có nguy cơ thấp bị RL huyết động và không có bằng chứng nhiễm trùng. Có thể kèm theo là triệu chứng “hết nghén”.

> EPL: Ra huyết thường gặp hơn đau bụng.

Đau bụng: thường dữ dội nhất trong lúc tống xuất mô thai, mức độ đau thay đổi từ nhẹ đến nặng, có thể đau liên tục hoặc từng cơn.

Sẩy thai có biến chứng: thường gặp nhất là sốc mất máu và nhiễm trùng. Nguy cơ tăng dần theo tuổi thai lúc sẩy. Nhiễm trùng này có khi là nhiễm trùng bậy bậy thôi, cũng có khi là sốc NT.

Lưu ý: thai phụ đã từng sinh con có thể khám thấy CTC mở kể cả trong 1 thai kỳ bth.

## Thai lưu

1 thai đã ngưng phát triển còn nằm trong tử cung.

Missed miscarriage: thai lưu không có biểu hiện lâm sàng mà chỉ chẩn đoán qua siêu âm.

- Tư vấn CDTK

## Dọa sẩy thai lưu - Threatened miscarriage.

Thuật ngữ có nghĩa là dự báo sẽ sẩy thai trên 1 thai lưu hoặc 1 thai khả năng rất cao là thai lưu. Dùng cho thai phụ ra huyết 3 tháng đầu với thai trong tử cung nhưng chưa có chẩn đoán thai lưu.

LS: ra máu, đau bụng, CTC đóng.

1 số dấu hiệu dự báo cao, nhưng chưa được kết luận là EPL:

Lặp lại siêu âm sau 7-10 ngày để xác lập chẩn đoán hoặc tư vấn chấm dứt thai kỳ cho bà mẹ.

## Sẩy thai khó tránh

Thuật ngữ: khả năng cao sẽ tống xuất thai lưu hoặc thai sống. Dùng trong TH CTC đang mở và ra huyết đang diễn tiến (đang sẩy).

LS: ra máu, CTC mở

## Sẩy thai không trọn

Sẩy thai nhưng vẫn còn mô trong tử cung. Dùng trong TH đã tống xuất khối mô nhưng chưa hoàn toàn hoặc thai lưu nằm dai dẳng trong tử cung.

LS: ra máu (rỉ rả kéo dài), đau quặn bụng, CTC hé mở

Giai đoạn sớm của sẩy thai không trọn có biểu hiện mở CTC, đau bụng còn tiến triển và có thể thấy 1 khối mô khi khám mỏ vịt. Giai đoạn sau, khi mà túi thai có thể vỡ ra, mô thai có thể bị tống xuất rồi, nhưng những phần còn lại (bánh nhau, màng rụng…) vẫn còn, khi đó thì triệu chứng sẽ giảm, siêu âm có thể thấy còn sót lại 1 khối mô hỗn hợp trong lòng TC, đặc biệt nếu SA doppler thấy tăng lưu lượng máu đến khối mô đó sẽ hướng nhiều chẩn đoán đến khối mô tống xuất chưa trọn.

## Sẩy thai trọn

Tống xuất thai hoàn toàn. Dùng để chỉ TH thai phụ đã biết có thai trong lòng tử cung trước đó và hiện tại lòng tử cung trống trên SA.

LS: ra máu nhiều, thấy 1 khối mô tống ra, CTC đóng.

## Chẩn đoán

Chẩn đoán thai nghén thất bại sớm được xác lập khi 1 thai kỳ đã xác định là có thai trong lòng tử cung trước đó, và siêu âm hiện tại thấy thai lưu trong tử cung hoặc buồng tử cung trống. (Uptodate, không thấy bất kỳ nguồn nào chỉ dựa vào lâm sàng mà chẩn đoán).

Nghi ngờ (cột bên phải) 🡪 lặp lại SA sau 7-10 ngày.

Độ chắc chắn của chẩn đoán tùy thuộc vào mong muốn giữ thai của bà mẹ (CRL ≥ 5mm + không tim thai hoặc GS ≥ 16mm + không phôi cũng có thể đủ để chẩn đoán cho bà mẹ muốn CDTK sớm)

- [x] tiêu chuẩn epl
> ![[IMG-20250504124024375.png]]


- [ ] Nguye cơ sảy
      ![[IMG-20250504124108678.png]]
## Xử trí thai nghén thất bại sớm

**Nguyên tắc**: phải chắc chắn chẩn đoán phân biệt được EPL với thai ngoài tử cung và thai trứng trước khi điều trị. Lựa chọn phương pháp nào là hoàn toàn tùy thuộc vào người bệnh.

> 1.**Theo dõi diễn tiến EPL**: chỉ nên áp dụng cho thai lưu < ==8 tuần==.
<!--SR:!2025-05-07,1,232--> 

Tỉ lệ thành công tới 80% nói chung và tới 90% với sẩy thai không trọn, dù phải theo dõi lặp lại nhiều lần. Theo dõi: bằng siêu âm, đáp ứng khi lòng tử cung không thấy túi thai và bề dày NMTC < 30mm (hoặc theo dõi bằng hCG, đáp ứng khi hCG giảm 80% trong 1 tuần sau khi tống xuất 1 khối …).

> Uptodate: nếu sau 4 tuần mà chưa tống xuất trọn khối thai, nên thay đổi phương pháp điều trị.

Misoprostol (Prostaglandin E1) 400mg hoặc 800mg (800mg cho liều khởi đầu, lặp lại – nếu cần thiết – với 400mg, ít tác dụng phụ hơn) đặt âm đạo gây co bóp tử cung mạnh, nhằm tống xuất thai lưu hoặc trứng trống. Tỉ lệ thành công tới 84% sau liều thứ 2.

ACOG: Misoprostol 800mg đặt âm đạo khởi đầu, lặp lại trong vòng 3h - 1 tuần sau liều đầu. Nếu có Mifepristol (U), nên dùng 24h trước liều Misoprostol.

Theo dõi đáp ứng: qua TVS.

Biến chứng:

- Tống xuất sót mô thai
- Nhiễm trùng
- Sốc mất máu
- Chỉ xảy ra trong TCN2: vỡ tử cung, chấn thương cổ tử cung

> 2.**Điều trị ngoại khoa**: hút lòng tử cung lấy thai lưu hoặc trứng trống. Thực hiện nhanh, ít mất máu, thành công tới 99%, nhưng có nguy cơ gây nhiễm trùng hoặc thủng tử cung.

> **Ưu thế trong lựa chọn PP điều trị**: LỰA CHỌN CỦA BN

- Theo dõi: dành cho thai phụ ngại dùng thuốc hoặc nạo hút, thai phụ phải dễ dàng theo dõi và can thiệp sau đó. Nhược điểm là phải chịu ra huyết và đau trằn bụng kéo dài.
- Nội khoa: BN có bất thường cấu trúc tử cung, gây khó tiếp cận cho dụng cụ chọc hút; BN muốn nắm rõ thời điểm sẩy thai hơn (vd như 1 bà mong con lớn tuổi rồi ko biết chờ thì tới chừng nào). Nhược điểm là đau bụng và ra huyết dữ dội hơn.
- Ngoại khoa: BN huyết động không ổn định hoặc có bệnh lý huyết học, đông máu thì nên làm thủ thuật cho gọn lẹ, tránh mất máu rỉ rả; hoặc BN muốn chấm dứt nhanh, tương tự như TH nội khoa. Nhược điểm là nguy cơ từ thủ thuật: NT, thủng tử cung.

> Theo dõi điều trị qua siêu âm hoặc B-hCG (nếu ko có SA) lặp lại mỗi ==1-2== tuần.
<!--SR:!2025-05-09,3,252-->

## Khuyến cáo của ACOG về EPL

Chứng cứ mức A:

- [ ] Đối với thai phụ được chỉ định điều trị nội khoa, khuyến cáo khởi đầu với 800 mg ==Misoprostol== đặt âm đạo, lặp lại nếu cần thiết.
      Bổ sung Mifepristone 200 mg (U) 24h trước liều Misoprostol giúp gia tăng đáng kể hiệu quả điều trị và nên cân nhắc dùng nếu có thể.
- Việc sử dụng thuốc chống đông, aspirin không làm giảm nguy cơ EPL ở phụ nữ mắc thrombophilias, trừ trường hợp mắc hội chứng anti-phospholipid
<!--SR:!2025-05-09,3,252-->

Mức chứng cứ B:
- Siêu âm là phương pháp được ưu tiên trong việc xác định có thai trong tử cung

> Không cần phải can thiệp ngoại khoa đối với phụ nữ có NMTC dày sau điều trị EPL nếu không có triệu chứng.
   Việc nạo hút lòng tử cung thường quy trong 3 tháng đầu thai kỳ không mang lại bất kỳ lợi ích nào, nếu như BS sản phụ khoa tự tin rằng lòng tử cung trống.

Mức chứng cứ C:

- Những phương pháp điều trị EPL được chấp thuận bao gồm theo dõi, nội khoa, ngoại khoa. Đối với phụ nữ không có tiền căn biến chứng sau điều trị nội khoa và không cần điều trị ngoại khoa khẩn trương, có thể lựa chọn phương pháp điều trị dựa theo ý muốn.

> Khuyến cáo sử dụng 1 liều duy nhất ==Doxycycline== để phòng ngừa nhiễm trùng sau khi điều trị ngoại khoa cho EPL
- Mặc dù nguy cơ xảy ra bất tương hợp máu mẹ con thấp nhưng hậu quả có thể rất nghiêm trọng và nên cân nhắc sử dụng globulin miễn dịch Rh-D trong các trường hợp EPL, đặc biệt là những trường hợp sảy thai muộn.
- Do nguy cơ mẫn cảm cao hơn, những phụ nữ có Rh-D âm tính được điều trị ngoại khoa nên được dự phòng bằng Ig Rh-D.
<!--SR:!2025-05-09,3,252-->

# Động học hCG và các vấn đề liên quan

hCG là glycoprotein (36k-40k Da) gồm 2 chuỗi alpha (92 aa, NST 6) và beta (145 aa, NST 19), trong đó đặc tính sinh học phụ thuộc vào chuỗi beta (beta-hCG giống  beta-LH tới 121 aa), còn chuỗi alpha là giống nhau giữa các hormone sinh dục. Nếu alpha và beta ko kết hợp, hCG ko thể gắn lên thụ thể LH.

hCG là hormone có nhiều lk carhohydrate nhất, vì vậy t½ của nó lên tới ==36==h.
<!--SR:!2025-05-09,3,252-->

Trong thai kỳ, hCG đc sx bởi hội bào nuôi -> đây là dấu hiệu có thai sinh hóa.

Ngoài ra hCG còn có thể đc sx từ thận, tuyến yên, 1 số mô khác của thai; tuyến yên ở người trưởng thành. hCG cũng đc tìm thấy trong bệnh lý tân sinh nguyên bào nuôi và vài bệnh lý ác tính khác.

Trong quá trình động học, hCG có nhiều dạng (do phân ly và đứt gãy): non-nicked hCG (hCG toàn phần không đứt gãy), nicked hCG (hCG toàn phần đứt gãy), free α-hCG (α-hCG tự do), non-nicked free β-hCG (β-hCG không đứt gãy, tự do), nicked free β-hCG (β-hCG đứt gãy, tự do), β-core fragment (mảnh vỡ lõi βhCG). Tỉ lệ các dạng này thay đổi theo tuổi thai (càng lớn tuổi thì tỉ lệ đứt gãy càng cao).

hCG có vai trò biến hoàng thể chu kỳ thành hoàng thể thai kỳ và duy trì nó, sx hormone steroid để nuôi dưỡng NMTC. Ngoài ra, hCG còn kích thích tinh hoàn thai nhi sx testosterone, do trước 110 ngày tuổi (15-16 tuần), tuần hoàn cửa tuyến yên chưa hình thành, nên tb Leydig sử dụng hCG từ lá nuôi thay cho LH từ tuyến yên của thai. Ngoài ra còn giúp thư giãn cơ trơn tử cung thông qua P4 và relaxin.

> hCG xuất hiện sau khi phôi làm tổ ==1== ngày (phôi 23-25 ngày tuổi). Nồng độ tăng gấp đôi mỗi 2 ngày đến tuần 6, đạt đỉnh vào tuần 8-10 (khoảng 100.000 mUI/mL). Sau đó nồng độ giảm dần và đạt cực tiểu vào tuần 16-20, duy trì đến cuối thai kỳ.
<!--SR:!2025-05-09,3,252-->

> Ngưỡng test QS (+): ==5== mUI/mL
<!--SR:!2025-05-09,3,252-->

## Ý nghĩa của hCG

Khi hCG đạt mức 1500, thì siêu âm đầu dò âm đạo thường có tể phát hiện GS trong buồng tử cung. Nếu không, phải nghĩ đến thai ngoài tử cung, thai ngưng tiến triển hoặc sẩy thai giai đoạn sớm.

Khi đạt mức 4000, có thể thấy được hoạt động tim phôi.

Khi đạt mức 5000-6000 có thể thấy GS qua siêu âm đầu dò bụng.

hCG cao bất thường ko tương xứng với tuổi thai có thể liên quan đến bệnh lý nguyên bào nuôi, đa thai hoặc tán huyết ở thai. hCG thấp bất thường hoặc tăng với tốc độ khác với dự đoán gợi ý thai kỳ thất bại sớm.

Trong trường hợp thai ngoài tử cung, có thể chọn test hCG bất kỳ, tuy nhiên khi theo dõi thì cần chọn cùng 1 dạng hCG giữa các lần.

Trong bệnh lý nguyên bào nuôi, nếu là thai trứng thì hCG toàn phần tăng nhanh, nếu là choriocarcinoma thì nicked β-hCG và non-nicked β-hCG là thành phần chính gia tăng.

Trong trường hợp thai lệch bội, nicked β-hCG chiếm tỉ trọng lớn và nói chung nicked β-hCG tăng trong các thai kỳ bệnh lý.

# Thai ngoài tử cung (Ectopic Pregnancy)

**Định nghĩa:** Khi thai làm tổ bên ngoài buồng tử cung.

Một số YTNC ảnh hưởng tới thai ngoài tử cung

1. Viêm nhiễm phụ khoa ảnh hưởng tới vòi trứng, đặc biệt do di chứng **Chlamydia trachomatis** ( gây viêm nhiễm và tổn thương trong ống dẫn trứng, làm thay đổi cấu trúc và chức năng của chúng)
2. Tiền sử phẫu thuật vòi trứng: (có thể gây tổn thương, sẹo gây chít hẹp vòi trứng)
3. Tiền sử thai ngoài tử cung (có thể là dấu hiệu của vấn đề cấu trúc hoặc chức năng với ống dẫn trứng, làm tăng nguy cơ xảy ra tình trạng tương tự trong tương lai)
4. Hút thuốc lá: Hút thuốc có thể làm giảm chức năng của lông nhung trong ống dẫn trứng, làm chậm quá trình di chuyển của trứng, và có thể dẫn đến việc trứng làm tổ ngoài tử cung.
5. Các kĩ thuật hỗ trợ sinh sản: kích thích rụng trứng, thụ tinh ống nghiệm và chuyển phôi (các phương pháp này có thể tăng số lượng trứng được thụ tinh, đôi khi làm tăng nguy cơ một trong số chúng làm tổ ngoài tử cung) 🡪 xác định sớm vị trí thai sau hỗ trợ sinh sản buộc tiến hành thường quy
6. Bất thường giải phẫu vòi trứng: polyp, túi thừa
7. Tránh thai khẩn cấp dùng progestin: (note cuối sách: Thuốc ngừa thai khẩn cấp chỉ chứa progestin không được xác nhận là YTNC gây thai ngoài tử cung. Tuy vậy phải tìm cách loại trừ khả năng thai ngoài tử cung khi bị thất bại khi dùng thuốc này)

Trong 3 thàng đầu thai kì bình thường, β-hCG huyết thanh tăng dần theo hàm số mũ. Trong vài tuần đầu của thai trong tử cung bình thường, 66% β-hCG tăng gấp đôi sau mỗi 2 ngày và không bao giờ tăng < 53% mỗi 2 ngày -> Nếu β-hCG tăng < 53% mỗi 2 ngày nên nghĩ tới khả năng

1. Thai trong tử cung với diễn tiến bất thường
2. Thai ngoài tử cung

Sau khi sảy thai tự nhiên, β-hCG huyết thanh sẽ giảm ít nhất 21-35% ,mỗi 2 ngày-> vì vậy, nếu β-hCG giảm chậm, < 20% mỗi 2 ngày thì nghĩ đến:

1. Còn tồn tại sản phẩm thụ thai
2. Có thai ngoài tử cung

Ngưỡng β-hCG phân định thường dùng là 1500-2000 mUI/mL để có thể thấy túi đơn thai trong lòng tử cung và ngưỡng này tăng lên 3000 mUI/mL so với song thai. Khi không thấy hình ảnh túi thai trong buồng tử cung và nồng độ β-hCG trên ngưỡng phân biệt, thì phải nghĩ đến khả năng có thai ngoài tử cung

Khi nồng độ β-hCG nằm dưới ngưỡng cắt và không thấy hình ảnh túi thai trong lòng tử cung -> “thai không xác định vị trí” (PUL - Prenancy of Unkhown Location)

## Uptodate

[**](https://www.uptodate.com/contents/ectopic-pregnancy-clinical-manifestations-and-diagnosis?search=ectopic%20pregnancy&source=search_result&selectedTitle=1~150&usage_type=default&display_rank=1#H153800166)[https://www.uptodate.com/contents/ectopic-pregnancy-clinical-manifestations-and-diagnosis?search=ectopic pregnancy&source=search_result&selectedTitle=1~150&usage_type=default&display_rank=1#H153800166**](https://www.uptodate.com/contents/ectopic-pregnancy-clinical-manifestations-and-diagnosis?search=ectopic%20pregnancy&source=search_result&selectedTitle=1~150&usage_type=default&display_rank=1#H153800166**)

🡪 Dấu hiệu chẩn đoán chắc chắn nhất TNTC là có túi thai có yolk sac/phôi (có/ không có tim thai ngoài TC)

Còn nếu siêu âm thấy túi thai trong lòng tử cung là đc rồi, lí do là bởi vì cái vòng đôi ở gần buồng trứng thì nó còn có thể là 1 cái hoàng thể, có thể nhìn nhầm

Nếu có túi thai mà không kèm yolksac/phôi thì cũng không chắc chắn chẩn đoán

Độ nhạy và đặc hiệu của SA+ cut off hCG >2000 để chẩn đoán TNTC là 10.9-95.2%Nghe theo giải đáp thắc mắc Y20: thì nhìn thấy hình ảnh yollsac nhưng chưa chắc đó là yolksac, phải làm gpb mới biết chính xác được. Nên dấu hiệu chắc chắn nhất TNTC là có tim thai

**Những hình ảnh có thể gợi ý (không phải chẩn đoán TNTC)**

- Khối phản âm hỗn hợp ngoài buồng tử cung
- Khối phản âm trống ngoài buồng tử cung

## Thai ngoài tử cung ở vòi trứng

**Diễn tiến**:

1. Vỡ vòi trứng (gây xuất huyết nội, là cấp cứu phụ khoa)
2. Sẩy qua loa vòi
3. Thoái triển (do giảm lượng máu tới thai)

**Tam chứng kinh điển trong thai ngoài tử cung ở vòi trứng**:

1. Đau hạ vị (99%)
2. Trễ kinh (75-90%)
3. Ra máu âm đạo bất thường (56%) : từ rĩ rả đến ra máu nhiều như máu kinh do (1) hCG thấp không đủ duy trì hoàng thể thai kì -> thiếu hụt estrogen và progesteron dẩn đến nội mạc tử cung bong tróc, (2) máu từ vòi trứng rỉ vào buồng tử cung

**Khám**: sờ được khối cạnh tử cung < 50% TH, có thể sờ được khối bên cạnh tử cung vì khối này là hoàng thể thai kì. Tử cung thường mềm và hơi to

**CLS**: SA thấy nội mạc dày do phản ứng Arias-Stella (PỨ mô học của nộ mạc tử cung với β-hCG), ít dịch ở cùng đồ Douglas

1. Theo dõi tới khi nó tự thoài triển hoàn toàn
2. Điều trị nội khoa bằng Methotrexate
3. Điều trị ngoại khoa

80% thai ngoài tử cung có β-hCG ≤ 1.000 mUI/mL sẽ không vỡ tự nhiên hoặc không chảy máu vào ổ bụng nhiều mà thường thoái triển tự nhiên.

**Theo dõi**: tới khi nó tự thoài triển hoàn toàn

Chỉ áp dụng cách xử trí này khi đẩy đủ các tiêu chuẩn sau đây:

1. BN có huyết động học ổn định
2. Siêu âm có kích thước khối thai ngoài tử cung < 2cm
3. β-hCG < 1000 mUI/mL và giảm dần theo thời gian (định lượng β-hCG hàng tuần tới khi âm tính)

**Điều trị nội khoa bằng Methotrexate**

Khi thỏa đầy đủ các điều kiện sau:

1. Huyết động học ổn định
2. Thai ngoài tử cung chưa vỡ
3. Kích thước khối thai < 3,5 cm và không có tim thai
4. β-hCG < 5000mUI/mL
5. BN có mong muốn điều trị nội khoa

Điều trị với MTX là chống chỉ định khi có 1 trong những yếu tố sau: (phải điều trị ngoại; khồng dùng MTX đc; phải theo dõi sát)

- Huyết động học không ổn định
    
- Thai ngoài tử cung vỡ
    
- Có bệnh lý huyết học như BC < 3000/ mm, tiểu cầu < 100000/mm hoặc suy chức năng gan, thận không cho phép dùng MTX (creatinin tăng, hoặc AST, ALT tăng)
    
    3
    
    3
    
- Bệnh lý loét dạ dày, bệnh phổi tiến triển hoặc suy giảm MD
    
- Quá mẫn với MTX
    
- Đang cho con bú hoặc có thai trong tử cung cùng tồn tại với thai ngoài tử cung, thường thấy sau sinh sản hỗ trợ với nhiều phôi
    
- Bệnh nhân không có thời gian làm xét nghiệm theo dõi β-hCG huyết thanh tới khi âm tính
    
- Khoảng cách nhà xa BV (sợ vỡ tử cung không cấp cứu kịp)
    
- BN không muốn điều trị nội khoa
    

Cơ chế hoạt động MTX: ức chế enzyme dihydrofolate reductase (DHFR), enzyme này chuyển đổi dạng không hoạt động của folate (dihydrofolate, DHF) thành dạng hoạt động (tetrahydrofolte, THF). THF là yếu tố cần thiết trong quá trình tổng hợp purin và thymidine, là các thành phần quan trọng của DNA 🡪 ức chế DHFR sẽ ức chế tổng hợp nguyên bào nuôi, và dùng MTX sẽ gây thiếu folate dạng hoạt động .

Trước khi bắt đầu tiêm MTX, BN dc xét nghiệm β-hCG huyết thanh, CTM, chức năng gan, thận để theo dõi diễn tiến và loại trừ CCĐ

Khi điều trị MTX BN sẽ được tiêm bắp MTX, liều 50 mg/m2 da. Trong khi điều trị MTX nên hướng dẫn BN:

- Tránh thức ăn chứa folate, tránh dùng NSAIDs vì thuốc này có thể tượng tác với MTX gây ức chế tủy xương, gây độc đường tiêu hóa.
- Tránh giao hợp vì có thể gây vỡ khối thai ngoài tử cung.
- Nên ngừa thai ít nhất 3 tháng sau khi β-hCG âm tính vì còn phải theo dõi đáp ứng đtrị.
- Hạn chế thăm khám âm đạo vì có thể gây vỡ thai ngoài TC.
- Tránh tiếp xúc với ánh sáng mặt trời vì có thể gây viêm da

Phác đồ điều trị đa liều MTX phải dùng thêm leucovorin xen kẽ để giảm thiểu tác dụng phụ do thiếu folate. So với phác đồ đa liều, phác đồ đơn liều hiệu quả hơn và ít tác dụng phụ hơn

Đánh giá vào ngày thứ 4 và thứ 7 sau tiêm, và sau đó là hằng tuần để đánh giá điều trị

- Ngày 7 giảm > 15% so với N4 🡪 có đáp ứng với MTX 🡪 định lượng β-hCG hàng tuần
- Ngày 7 giảm < 15%, hay tăng hay bình nguyên so với N4 🡪 không đáp ứng MTX L1 🡪 MTX liều 2 nếu còn chỉ định

Siêu âm để đánh giá lượng dịch tự do trong ổ bụng đối với BN đau bụng nhiều nghi thai ngoài tử cung vỡ sau điều trị MTX. Thường đau bụng sau vài ngày tiêm MTX chủ yếu do khối thai sẩy qua loa ngoài/ máu tụ làm vòi trứng căng (Không nên sd siêu âm làm phương tiện theo doi điều trị MTX vì SA sẽ thấy khối thai to lên do khối máu tụ chứ ko phải thất bại điều trị MTX)

Khi huyết động bất thường 🡪 mổ mở. Nếu huyết động ổn định và dụng cụ sẵn có, vẫn có thể mổ nội soi

**Điều trị ngoại khoa**

Khi thai ngoài tử cung chưa vỡ, điều trị nội khoa là bình đẳng với điều trị ngoại khoa

Các tình huống điều trị ngoại kho là bắt buộc hay thiên lệch về điều trị ngoại khoa

- Thai ngoài tử cung đã vỡ hoặc chưa vỡ nhưng huyết động không ổn định
- CCĐ dùng MTX
- Điều trị MTX thất bại
- Có bệnh hiếm muộn nguyên nhân vòi trứng cần cắt bỏ và có kế hoạch làm thụ tinh trong ống nghiệm
- Có thai trong tử cung cùng tồn tại
- Mong muốn triệt sản

Cách mổ có thể là cắt vòi trứng toàn phần hoặc xẻ vòi trứng bảo tồn

Cắt vòi trứng toàn phần là can thiệp triệt để:

Phẫu thuật này được thực hiện cho các trường hợp sau

- Tổn thương nặng vòi trứng
- Thai ngoài tử cung vỡ
- Thai ngoài tử cung tái phát ở vòi trứng cùng bên
- Khối thai ngoài to > 5cm
- BN không muốn có thai trong tương lai

Xẻ vòi trứng bảo tồn: trong trường hợp BN còn muốn có thai trong tương lại, tuy nhiên, khả năng này phụ thuộc vào tỷ lệ tổn thương ống dẫn trứng

Nguy cơ sót nguyên bào nuôi khoảng 3-20% 🡪 cần định lượng β-hCG sau mổ 3 ngày

- Giảm > 20% so với trước mổ: 🡪 thành công 🡪 định lượng hàng tuần đến khi âm tính
- Giảm < 20% so với trước mổ 🡪 sót nguyên bao nuôi 🡪 điều trị MTX 50 mg tiêm bắp

Nên tư vấn kỹ cho bệnh nhân về tương lai sản khoa vì nếu người đã bị 1 lần thai ngoài tử cung thì nguy cơ bị thai ngoài tử cung trong tương lai tăng lên 7-13 lần, khả năng có thai ở lần có thai tiếp theo là: 50-80% có thai trong tử cung và 10-25% thai ngoài tử cung

# XHTC 3 tháng đầu thai kì

Quản lý qua 3 câu hỏi:

1. Có thai hay không?
2. Thai làm tổ ở đâu?
3. Sinh tồn của thai?

Các chẩn đoán phân biệt:

- Thai ngoài tử cung
- Thai nghén thất bại sớm
- Sẩy thai không trọn
- Song thai biến mất
- Bất thường âm đạo/cổ tử cung: rách, bướu, mụn cóc, viêm nhiễm,...
- Chẩn đoán loại trừ: dọa sẩy thai, rong kinh, chảy máu do làm tổ…

## TVS là khảo sát đầu tay

Siêu âm qua đường âm đạo (Transvaginal Ultrasound Scan - TVS) là khảo sát sơ cấp được chọn. So với SA qua đường bụng, SA qua âm đạo có độ phân giải tốt hơn, phân biệt chi tiết có kích thước mm. Nhược điểm: có tầm quan sát hạn chế

2 thông tin mà TVS có thể mang lại:

1. Sinh tồn trứng
2. Hình ảnh túi thai trong tử cung

_Hình ảnh túi thai trong tử cung:_ khi kết thúc tuần 5, đã có thể thấy túi thai trên SA -> hiện diện túi thai trong TC hướng chấn đoán về thai nghén thất bại sớm, trừ trường hợp túi thai giả, song thai với 1 thai trong và 1 thai ngoài tử cung)

Khi túi thai không được nhìn thấy qua TVS , chỉ có thể kết luận không thấy túi thai qua TVS, mà không được kết luận TNTC trừ trường hợp thấy được túi thai bên ngoài tử cung với quầng nguyên bào nuôi, yolk-sac, có/không có phôi thai với hoạt động tim thai

Thai trứng toàn phần: HẢ điển hình tổ ong của các gai nhau bị thoái hóa nước. Trong thai trứng bán phần, hình ảnh ko còn rõ ràng. Thai lưu với nhau thoái hóa sẽ cho hình ảnh tương tự thai trứng

Chọn siêu âm Doppler ưu thế hơn grey scale

## Định lượng thứ cấp là β-hCG

Trong 3 thàng đầu thai kì bình thường, β-hCG huyết thanh tăng dần theo hàm số mũ. Trong vài tuần đầu của thai trong tử cung bình thường, 66% β-hCG tăng gấp đôi sau mỗi 2 ngày và không bao giờ tăng < 53% mỗi 2 ngày 🡪 Nếu β-hCG tăng <53% mỗi 2 ngày nên nghĩ tới khả năng

1. Thai trong tử cung với diễn tiến bất thường
2. Thai ngoài tử cung

Sau khi sảy thai tự nhiên, β-hCG huyết thanh sẽ giảm ít nhất 21-35%, mỗi 2 ngày 🡪 vì vậy, nếu β-hCG giảm chậm, < 20% mỗi 2 ngày thì nghĩ đến:

1. Còn tồn tại sản phẩm thụ thai
2. Có thai ngoài tử cung

Tuy nhiên nếu chỉ dựa vào động học β-hCG thì khảo sát thai ngoài tử cung sẽ bị hạn chế

- Khái niệm ngưỡng phân định β-hCG và cut off của nó. Nếu β-hCG trên ngưỡng phân định này, khả năng hình thấy túi thai trong tử cung có độ đặc hiệu cao. Nếu β-hCG dưới ngưỡng phân định, khả nặng bỏ sót thai ngoài tử cung có độ nhạy thấp

Ngưỡng β-hCG phân định thường dùng là 1500-2000 mUI/mL để có thể thấy túi đơn thai trong lòng tử cung và ngưỡng này tăng lên 3000 mUI/mL so với song thai. Khi không thấy hình ảnh túi thai trong buồng tử cung và nồng độ β-hCG trên ngưỡng phân biệt, thì phải nghĩ đến khả năng có thai ngoài tử cung

Khi nồng độ β-hCG nằm dưới ngưỡng cắt và không thấy hình ảnh túi thai trong lòng tử cung 🡪 “ thai không xác định vị trí” (PUL - Prenancy of Unkhown Location)

Thời gian làm lại β-hCG (note giải đáp thắc mắc Y19)

**VD**: BN trễ kinh, quick-test (+), có chảy máu âm đạo, nhưng tính tuổi thai cỡ 5 tuần thì làm sao?

BN có chu kì kinh nguyệt đều 🡪 BS thấy tuổi thai còn nhỏ 🡪 ra về hẹn 2 tuần sau tái khám

Chu kì kinh nguyệt không đều 🡪 ưu tiên TVS

- Nếu SA thấy túi thai trong lòng tử cung 🡪 không làm β-hCG nữa
- Hình ảnh gợi ý TNTC (nội mạc mỏng 5-6mm, có khối echo trống ngoài tử cung)

Lưu ý: không phải thấy khối echo trống ngoài TC là TNTC, chắc chắn nhất là thấy hình ảnh yolk-sac, phôi thai ngoài TC

- Nếu không thấy túi thai làm β-hCG
- Nếu quá thấp so với ngưỡng phân định (VD cỡ 200) 🡪 hẹn tài khám sau 1 tuần, vì làm định lượng sau 48h nữa cũng không đặt DZ
- Nếu gần mức DZ thì nên làm lại β-hCG sau 48h nữa do chưa loại trừ trường hợp song thai hay bệnh nội mạc vùi trong cơ làm khó thấy hình ảnh thai
- DZ > 3000 🡪 vượt quá ngưỡng song thai 🡪 chắc chắn TNTC và điều trị

## Lưu đồ tiếp cận

## Lâm sàng

Dọa sẩy thai: ra máu, đau bụng, CTC đóng

Sẩy thai khó tránh: ra máu, CTC mở

Sẩy thai không trọn: ra máu (rỉ rả kéo dài), đau quặn bụng, CTC hé mở

Sẩy thai trọn: ra máu (nhiều), CTC đóng, tử cung nhỏ, thấy 1 khối lạ đc tống xuất.

TNTC: đau bụng, ra máu (rỉ rả hoặc như rong kinh), tử cung mềm và hơi to

## Siêu âm

Dọa sẩy thai: thấy thai trong tử cung với nhiều dấu hiệu dự báo

Sẩy thai khó tránh: thấy thai đang trên đường tống xuất khỏi tử cung (cần phân biệt với TNTC ở vị trí CTC, dùng Beta HCG)

Sẩy thai không trọn: thấy còn sót 1 phần thai trong tử cung

Sẩy thai trọn: tử cung trống

TNTC: nội mạc mỏng, tử cung trống, có thể thấy khối ngoài tử cung

## B-hCG

Dọa sẩy thai, sẩy thai trọn/không trọn: B-hCG không có giá trị

Trường hợp ra huyết mà siêu âm thấy tử cung trống, thì B-hCG tụt giúp hướng đến chẩn đoán sây thai trọn hơn là TNTC

Sẩy thai khó tránh: B-hCG giúp phân biệt với trường hợp TNTC ở cổ tử cung

TNTC: động học B-hCG thay đổi chậm

Tại vì bà này 42 tuổi, sẩy thai 2 lần, thai thì đang dần chậm tăng trưởng -> hướng tới 1 ca EPL nên mới phải làm vầy.

Chứ nếu mà trong những ca bình thường, thì vẫn lấy kq SA tuần 10-13+6

Động học nó khác nhau sao?

Chảy máu nhiều r cầm máu sao ta?

hCG trong nước tiểu là loại nào

Theo mong muốn của ng bệnh là quan trọng nhất