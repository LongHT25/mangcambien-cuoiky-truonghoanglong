# Đồ án môn Mạng Cảm Biến: Phân loại âm thanh động vật
- **Thành viên thực hiện:** Trương Hoàng Long - N23DCCI043
- **Tên đề tài:** Nhận diện 4 loại âm thanh (Chó, Mèo, Gà, Chim) và Tiếng ồn bằng Spectrogram + 2D-CNN.

## Mô tả thư mục
- `index.html`, `run-impulse.js`: Giao diện Web thu âm thời gian thực.
- `edge-impulse-standalone.wasm`: Khối mô hình AI (WebAssembly).
- `server.py`: Script khởi chạy server cục bộ.

## Phụ thuộc (Dependencies)
- Python 3.x
- Trình duyệt web cấp quyền truy cập Microphone.

## Hướng dẫn cài đặt và chạy
1. Tải toàn bộ source code về máy.
2. Mở Terminal/Command Prompt tại thư mục chứa source code.
3. Chạy lệnh: `python -m http.server 8082` (đối với Windows) hoặc `python3 server.py`.
4. Truy cập trình duyệt tại địa chỉ: `http://localhost:8082`.