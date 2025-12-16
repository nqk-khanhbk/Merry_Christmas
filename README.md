# Magic Christmas (Kain Nguyen)

Hướng dẫn chạy demo Noel nhận diện cử chỉ tay (Mediapipe + Three.js) hiển thị cây thông, pháo hoa và bộ ảnh.

## Yêu cầu
- Trình duyệt hiện đại (Chrome/Edge) và cho phép dùng camera.
- Kết nối Internet để tải CDN (three.js, mediapipe).
- Chạy trên `localhost` (hoặc HTTPS) để camera hoạt động; không mở trực tiếp file `file://`.

## Cấu trúc thư mục
- `Merry_Christmas/`
	- `index.html`: bản cuối, nên chạy file này.
	- `audio.mp3`, `image1.jpeg` → `image5.jpeg`: nhạc nền và ảnh hiển thị.

## Cách chạy nhanh
1. Mở thư mục này trong VS Code.
2. Dùng một trong hai cách tạo server cục bộ tại thư mục `Merry_Christmas/`:
	 - **VS Code Live Server**: chuột phải `index1.html` → `Open with Live Server`.
	 - **Python** (nếu có):
		 ```bash
		 cd Merry_Christmas
		 python -m http.server 8000
		 ```
		 Sau đó mở `http://localhost:8000/index%20ver1.1.html`.
3. Trình duyệt sẽ hỏi quyền camera → bấm Allow.

## Cách dùng
- Nhấn nút **START MAGIC** để bật nhạc và hiệu ứng.
- Cử chỉ tay (đưa tay vào khung):
	- ✊ Nắm tay: chế độ **TREE** (cây thông, ngôi sao). 
	- 🖐 Xòe tay: **EXPLODE** (pháo hoa/ảnh xoay quanh).
	- 🫶 Hai tay chụm tim: **HEART** (hiện chữ I LOVE YOU).
	- Pinch ngón cái + trỏ: **PHOTO** (phóng to ảnh nổi bật).

## Mẹo
- Giữ các file ảnh/nhạc cùng thư mục với HTML để tránh lỗi tải tài nguyên.
- Nếu không thấy camera, đảm bảo truy cập bằng `localhost` và đã cấp quyền.
