# AI Office Operations - Prompt Library

Bộ prompt này chuyển các phương pháp trong 3 tài liệu đào tạo thành các mẫu có thể tái sử dụng.

## Prompt 0 - Prompt Builder 6 thành phần

Vai trò: Bạn là ...
Nhiệm vụ: Hãy ...
Bối cảnh: Mục đích / người đọc / tình huống là ...
Đầu vào: Dữ liệu tôi cung cấp gồm ...
Đầu ra: Trả kết quả dưới dạng ...
Ràng buộc: Không ... / tối đa ... / nếu thiếu dữ liệu thì ...

---

## Prompt 1 - Xử lý văn bản dài

Đọc tài liệu dưới đây.
Không bổ sung thông tin không có trong tài liệu.

1) Tóm tắt trong tối đa 150 từ.
2) Liệt kê 05 nội dung quan trọng nhất.
3) Lập bảng: Nội dung | Người/bộ phận liên quan | Thời hạn | Việc cần thực hiện.
4) Nếu tài liệu không nêu rõ thông tin, ghi "Chưa xác định".

Ràng buộc:
- Không thêm thông tin.
- Không tự tạo người, hạn, căn cứ hoặc kết luận.
- Giữ nguyên mức độ chắc chắn của nguồn.

---

## Prompt 2 - Soạn/chỉnh văn bản hành chính theo 2 vòng

### Vòng 1 - Trích xuất

Hãy đọc yêu cầu dưới đây và lập bảng gồm:
Nội dung | Người/đơn vị | Hạn | Yêu cầu đầu ra | Còn thiếu.

Không soạn văn bản ở bước này.
Đánh dấu [CẦN XÁC NHẬN] nếu thông tin mơ hồ hoặc mâu thuẫn.

### Vòng 2 - Sau khi người dùng xác nhận bảng

Dựa trên bảng đã được xác nhận, hãy soạn:
1) Email triển khai.
2) Thông báo nội bộ.
3) Bảng giao việc.

Giữ thống nhất người - việc - hạn - sản phẩm.
Không thêm căn cứ hoặc thông tin mới.

---

## Prompt 3 - Chuyển yêu cầu thành bảng giao việc

Bạn là trợ lý tổ chức công việc.

Hãy đọc yêu cầu tôi cung cấp và:
1) Chuẩn hóa danh sách đầu việc.
2) Gộp việc trùng và đề xuất tên việc chuẩn.
3) Đánh dấu việc mô tả mơ hồ.
4) Xác định người/đơn vị nếu nguồn có.
5) Ghi deadline nếu nguồn có.
6) Ghi sản phẩm đầu ra nếu nguồn có.
7) Đánh dấu phần thiếu bằng "Chưa xác định" hoặc "[CẦN BỔ SUNG]".
8) Lập bảng: STT | Việc | Chủ trì | Phối hợp | Deadline | Sản phẩm | Trạng thái.

Không tự tạo thông tin.

---

## Prompt 4 - Hỗ trợ nhân sự cơ bản

Bạn là trợ lý hỗ trợ hành chính nhân sự.

Từ ghi chú tuyển dụng dưới đây, hãy tạo 2 đầu ra:
1) Mô tả công việc nội bộ.
2) Tin tuyển dụng ngắn để đăng nội bộ.

Không tự thêm lương, địa điểm hoặc quyền lợi nếu chưa có.
Thiếu thông tin thì ghi [CẦN BỔ SUNG].

### Output 1 - JD nội bộ
- Mục tiêu vị trí.
- Nhiệm vụ.
- Yêu cầu.
- Trách nhiệm.
- Người báo cáo nếu nguồn có.
- Tiêu chí/điểm cần bổ sung nếu nguồn có.

### Output 2 - Tin tuyển dụng
- Tiêu đề.
- Mô tả ngắn.
- Yêu cầu.
- Cách nộp hồ sơ nếu nguồn có.

Không tự quyết tuyển/loại ứng viên.

---

## Prompt 5 - Danh sách việc thô -> kế hoạch tuần

Bạn là trợ lý tổ chức công việc.

Hãy chuẩn hóa danh sách việc, đánh dấu việc trùng/thiếu thông tin, phân nhóm P1/P2/P3, sau đó lập kế hoạch tuần từ Thứ 2 đến Thứ 6.

Yêu cầu:
- Không tự tạo deadline cho việc chưa có hạn.
- Gộp việc trùng nhưng không làm mất ý.
- Đánh dấu mô tả mơ hồ.
- Tách riêng:
  + Chờ thông tin
  + Chờ phản hồi
  + Chờ phê duyệt
- Không biến trạng thái chờ thành quá hạn.
- Kế hoạch tuần phải có: Ngày | Ưu tiên | Công việc | Deadline | Sản phẩm.
- Không tự thêm lịch cố định nếu nguồn không nêu.

---

## Prompt 6 - Transcript -> phân loại trước khi viết biên bản

Đọc transcript họp dưới đây.

1) Phân loại từng ý thành:
   - Ý kiến
   - Kết luận
   - Việc
   - Chưa chốt
2) Ghi người/đơn vị liên quan nếu nguồn nêu.
3) Ghi deadline nếu nguồn nêu.
4) Ghi rõ chỗ thiếu người, hạn hoặc căn cứ.
5) Không viết biên bản ở bước này.
6) Sau khi tôi xác nhận, mới tạo biên bản.

Quy tắc:
- "Đã thống nhất" khác "được đề xuất".
- Không tự xác định người chủ trì.
- Không tự tạo deadline.

---

## Prompt 7 - Biên bản -> bảng hành động

Dựa trên biên bản họp đã được xác nhận, hãy lập bảng:

STT | Việc | Chủ trì | Phối hợp | Hạn | Sản phẩm | Trạng thái.

Chỉ ghi người/hạn/trạng thái khi có căn cứ trong biên bản.
Thiếu thì ghi [CẦN XÁC NHẬN].

Sau bảng, liệt kê riêng:
- Nội dung chưa chốt.
- Việc thiếu người.
- Việc thiếu deadline.
- Điểm cần người có thẩm quyền xác nhận.

---

## Prompt 8 - Nhiều báo cáo -> báo cáo tổng hợp

Đọc các báo cáo tôi cung cấp.

### Bước 1 - Chuẩn hóa
Lập bảng:
Đơn vị | Việc chính | Trạng thái | Kết quả | Vướng mắc | Deadline | Việc tiếp theo.

### Bước 2 - Phát hiện lệch
Liệt kê:
- Điểm trùng.
- Khác số liệu.
- Khác trạng thái.
- Khác deadline.
- Thông tin chỉ xuất hiện ở một nguồn.
- Nội dung cần xác nhận.

### Bước 3 - Tổng hợp
Viết báo cáo 1-2 trang theo:
1) Tình hình chung.
2) Kết quả đã đạt.
3) Công việc đang triển khai.
4) Vướng mắc/rủi ro.
5) Nội dung cần xác nhận.
6) Nhiệm vụ kỳ tiếp theo.

Không "làm phẳng" dữ liệu.
Không tự chọn nguồn đúng khi các nguồn chưa thống nhất.
Không suy đoán nguyên nhân.

---

## Prompt 9 - Excel -> báo cáo tiến độ

Bạn là trợ lý theo dõi tiến độ.

Ngày báo cáo là [DD/MM/YYYY].

Phân tích bảng công việc và tạo:
1) Tổng số việc.
2) Số đã hoàn thành.
3) Số đang làm.
4) Số quá hạn.
5) Số đang chờ.
6) Danh sách việc quá hạn.
7) Việc sắp đến hạn theo quy tắc tôi cung cấp.
8) Việc đang chờ.
9) Dữ liệu bất thường.
10) Tóm tắt tối đa 7 câu.

Quy tắc:
- Quá hạn chỉ khi deadline trước ngày báo cáo và trạng thái chưa hoàn thành.
- Không tự tạo deadline.
- Không tự thay đổi trạng thái.
- Không tự sửa % tiến độ.
- Nếu trạng thái và % không khớp, chỉ đánh dấu bất thường.
- Trước khi phân tích, mô tả cách hiểu các cột và đơn vị nếu chưa rõ.

---

## Prompt 10 - Báo cáo -> tóm tắt lãnh đạo

Dựa trên báo cáo tổng hợp và phân tích tiến độ đã cung cấp, hãy viết tóm tắt phục vụ lãnh đạo theo 4 phần:

1) Thông tin.
2) Vấn đề.
3) Nguyên nhân có căn cứ.
4) Hành động tiếp theo.

Yêu cầu:
- Ưu tiên số liệu có căn cứ.
- Không biến suy luận thành nguyên nhân.
- Nếu chưa đủ dữ liệu: ghi "Chưa đủ căn cứ xác định nguyên nhân".
- Hành động phải rõ người - việc - hạn khi nguồn có.
- Nếu cần quyết định của lãnh đạo, đưa vào mục "Nội dung cần quyết định".

Độ dài: tối đa 1 trang hoặc khoảng 350-450 từ.

---

## Prompt QA - Phản biện đầu ra

Hãy kiểm tra đầu ra vừa tạo theo 5 tiêu chí:
1) Đúng.
2) Đủ.
3) Có căn cứ.
4) Đúng ngữ cảnh.
5) An toàn.

Sau đó trả:
- Lỗi phát hiện.
- Dòng/ý cần sửa.
- Căn cứ từ nguồn.
- Bản sửa thận trọng hơn.

Không dùng bản tự kiểm tra này để thay thế việc đối chiếu nguồn gốc.
