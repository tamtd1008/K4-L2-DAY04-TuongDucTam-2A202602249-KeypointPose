# Mini guideline - nhóm: G02 - T009  |  người gán: Tưởng Đức Tâm  |  ngày:16/09/2026

> Điền file này **trong lúc** gán nhãn, không phải sau khi xong. Mỗi lần bạn dừng lại
> hơn 10 giây để phân vân, đó là một dòng phải ghi vào đây.

## 1. Luật bắt buộc (đã thống nhất cả lớp - không sửa)

- Bộ 17 điểm COCO, đúng tên, đúng thứ tự. Lấy từ file `.SVG` chung.
- Mọi người trong ảnh đều có **đủ 17 điểm**. Điểm không dùng được thì gắn cờ, không xoá.
- Trái/phải tính theo **cơ thể người**, không theo bức ảnh.
- Bị che, còn trong khung -> `v = 1`, **vẫn đặt chấm** ở vị trí ước lượng.
- Ra ngoài mép ảnh -> `v = 0`, **không** đặt chấm.
- Không dùng `Hidden` (`h`) - nó không được lưu vào file.

## 2. Luật của nhóm bạn (phải điền)

| Tình huống | Luật nhóm bạn chọn | Vì sao |
| --- | --- | --- |
| Hông của người mặc quần áo dài |visibled | |
| Tai bị tóc hoặc mũ bảo hiểm che một phần |occluded | |
| Người bị cắt ở mép ảnh (chỉ thấy từ hông trở lên) |truncated | |
| Cổ tay nằm sau tay lái / sau thân mình |occluded | |
| Hai người chồng lên nhau |occluded | |
| Người nhỏ đến mức nào thì không gán nữa |không nhận định được rõ là người | |

Với mỗi luật, chèn **một ảnh mẫu** (screenshot từ CVAT) thay vì chỉ viết một câu.
Slide 12 nói rõ: khớp không có bề mặt nhìn thấy được thì phải có ảnh mẫu, không phải
một câu văn chung chung.

## 3. Ba ca mơ hồ đã gặp (bắt buộc, ghi ít nhất 3)

### Ca 1 - ảnh `train_03.jpg`, người thứ `___`, khớp `______`

- Mơ hồ ở chỗ nào: búp bê nằm dưới lòng đường có tính là người không
- Bạn quyết thế nào: không
- Vì sao: đâm xe vào búp bê nằm trên đường không gây hậu quả gì
- Nếu người khác quyết ngược lại thì model học sai cái gì: dừng xe lại nhiều hơn, gây phiền toái

### Ca 2 - ảnh `train_13.jpg`, người thứ `___`, khớp `______`

- Mơ hồ ở chỗ nào: 2 người ở phía sau bị mờ, khó nhận rõ bộ phận cơ thể
- Bạn quyết thế nào: vẫn xác định keypoint
- Vì sao: vẫn hiểu được đó là người
- Nếu người khác quyết ngược lại thì model học sai cái gì: dễ bỏ sót khi theo dõi hoạt động của người ở xa

### Ca 3 - ảnh `train_18.jpg`, người thứ `___`, khớp `______`

- Mơ hồ ở chỗ nào:bóng của người đi xe đạp
- Bạn quyết thế nào: không xác định keypoint
- Vì sao: bóng không phải vật thể, không phải người
- Nếu người khác quyết ngược lại thì model học sai cái gì: xác định thêm nhiều vật thể ảo

## 4. Sau khi so visibility report với bạn cùng nhóm

- Khớp lệch `%v=1` nhiều nhất: `______` (bạn `___%` / họ `___%`)
- Nguyên nhân là **guideline chưa rõ** hay **một trong hai bên gán sai**:
- Luật mới bổ sung vào mục 2 sau khi thống nhất:
