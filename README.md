# Đồ án môn Mạng Cảm Biến

- **Thành viên thực hiện:** Trương Hoàng Long - N23DCCI043
- **Tên đề tài:** Phân loại tiếng động vật quanh nhà (4 lớp) và tiếng ồn bằng Spectrogram kết hợp mạng 2D-CNN.

## Mô tả cấu trúc thư mục
- `index.html`: Giao diện Web thu thập âm thanh thời gian thực (tần số lấy mẫu 16000Hz).
- `edge-impulse-standalone.wasm` & `edge-impulse-standalone.js`: Khối mô hình AI (WebAssembly) đã được huấn luyện.
- `run-impulse.js`: Script hỗ trợ khởi tạo mô hình.
- `server.py`: Script khởi chạy máy chủ cục bộ (Localhost) để cấp đúng quyền MIME type cho tệp `.wasm`.

## Yêu cầu hệ thống (Dependencies)
- Python 3.x
- Trình duyệt web (Chrome, Edge, Safari...) có hỗ trợ và cho phép quyền truy cập Microphone.

## Hướng dẫn cài đặt và chạy thực nghiệm
1. Tải toàn bộ mã nguồn về máy tính.
2. Mở Terminal hoặc Command Prompt (CMD) tại thư mục chứa mã nguồn.
3. Khởi chạy máy chủ ảo bằng lệnh sau:
   ```bash
   python server.py (Lưu ý: Trên MacOS hoặc Linux, vui lòng sử dụng lệnh python3 server.py)
4. Mở trình duyệt web và truy cập vào địa chỉ: http://localhost:8082
5. Cấp quyền truy cập Microphone khi trang web yêu cầu và bắt đầu quá trình nhận diện.
