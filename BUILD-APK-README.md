# Cờ Vua — đóng gói HTML thành APK Android

Dự án này là một app Android tối giản, chỉ có một WebView tải file
`app/src/main/assets/index.html` (chính là file chess.com-style bạn
đang chỉnh) và hiển thị toàn màn hình. Không cần mạng, không cần API
key, không có màn hình Compose nào khác.

## Cách lấy file APK (không cần cài Android Studio)

1. Tạo một repository mới trên GitHub (public hoặc private đều được).
2. Tải toàn bộ nội dung file zip này lên repo đó (giữ nguyên cấu trúc thư mục).
3. Vào tab **Actions** của repo → chọn workflow **Build APK** → bấm **Run workflow**.
4. Đợi vài phút cho build xong (màu xanh ✅) → mở lần chạy đó ra → mục
   **Artifacts** ở cuối trang → tải **app-debug** (file `.zip` chứa
   `app-debug.apk` bên trong).
5. Chuyển file `app-debug.apk` vào điện thoại Android, mở lên cài
   (cần bật "Cài ứng dụng từ nguồn không xác định" cho trình duyệt/
   trình quản lý file bạn dùng để mở file này).

## Cách build trên máy (nếu có Android Studio)

1. Mở Android Studio → **Open** → chọn thư mục dự án này.
2. Để Android Studio tự đồng bộ Gradle.
3. Run ▶ trên máy ảo hoặc điện thoại thật.

## Cập nhật lại giao diện sau này

Muốn đổi giao diện app, chỉ cần thay nội dung file
`app/src/main/assets/index.html` bằng bản HTML mới, rồi build lại —
không cần sửa gì trong code Kotlin.
