[BTTH] Bài tập thực hành tổng hợp
# BÁO CÁO TỔNG HỢP: GIẢI PHÁP TỰ ĐỘNG HÓA CHĂM SÓC KHÁCH HÀNG

## 1. VẤN ĐỀ VÀ MỤC TIÊU
* **Vấn đề:** Khi khách hàng nhắn tin phàn nàn nhưng hay quên gửi mã đơn hàng, hệ thống dễ bị lỗi hoặc tự đoán sai sự thật.
* **Mục tiêu:** Xây dựng một quy trình tự động qua nhiều bước để lọc lỗi thông tin trước khi tiến hành giải quyết.

## 2. CÁCH THỰC HIỆN QUA 2 BƯỚC NỐI TIẾP
* **Bước 1 (Kiểm tra thông tin):** Đọc tin nhắn của khách và dữ liệu đơn hàng. Nếu thiếu mã đơn, hệ thống sẽ dừng lại và yêu cầu khách bổ sung ngay, không kiểm tra tiếp để tránh nhầm lẫn.
* **Bước 2 (Xử lý và trả lời):** Nếu thông tin đã đầy đủ, hệ thống sẽ tự động đối chiếu quy định (đổi trả trong 7 ngày) rồi soạn tin nhắn trả lời lịch sự cho khách.

## 3. KẾT QUẢ THỬ NGHIỆM THỰC TẾ
* **Tình huống:** Khách nhắn *"Sản phẩm bị lỗi, hoàn tiền ngay!"* (Quên gửi mã đơn).
* **Kết quả từ hệ thống:** 
  > **TRẠNG THÁI:** `[Cần bổ sung thông tin]`
  > 
  > **TIN NHẮN TRẢ LỜI:** Chào bạn, shop rất tiếc vì sự cố này. Để bên mình hỗ trợ hoàn tiền nhanh nhất, bạn vui lòng gửi lại giúp shop **Mã đơn hàng** nhé!
