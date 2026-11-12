# Gym Tracker PWA

Ứng dụng theo dõi tập luyện chạy trên trình duyệt, tối ưu cho iPhone. Có thể thêm vào màn hình chính như một app.

## Chạy thử trên Windows
1. Giải nén thư mục.
2. Mở PowerShell tại thư mục này.
3. Chạy `py -m http.server 8000`.
4. Trên máy tính mở `http://localhost:8000`.
5. Để mở trên iPhone cùng Wi-Fi: tìm IPv4 của máy Windows bằng `ipconfig`, sau đó mở `http://IP-MAY-TINH:8000` trên Safari.

## Cài lên màn hình chính iPhone
Để PWA cài đặt ổn định và Service Worker hoạt động, website cần được host bằng HTTPS (ví dụ GitHub Pages hoặc Netlify).
1. Đưa các file trong thư mục lên một repository GitHub.
2. Bật GitHub Pages trong Settings > Pages.
3. Mở URL HTTPS trên Safari iPhone.
4. Chọn Share > Add to Home Screen > Add.

## Tính năng
- Tạo buổi tập, thêm bài tập và ghi set/kg/rep/RIR.
- Lưu lịch sử trong localStorage của trình duyệt.
- Tính volume (kg × reps), thống kê tuần, PR và Estimated 1RM theo công thức Epley.
- Thư viện bài tập theo nhóm cơ và bài tập tùy chỉnh, có ảnh minh họa khi dữ liệu ảnh tương ứng tồn tại.
- Trang chi tiết bài tập với ảnh tư thế và liên kết tìm video hướng dẫn trên YouTube.
- Đồng hồ nghỉ giữa set: chọn 30–300 giây, bắt đầu/tạm dừng/đặt lại; tự chạy khi đánh dấu set hoàn thành.
- Biểu đồ volume tuần và tiến bộ theo bài.
- Light/Dark mode, xuất/nhập JSON để sao lưu.

## Lưu ý
- Dữ liệu lưu trên chính trình duyệt/thiết bị, không tự đồng bộ giữa máy tính và iPhone.
- Xuất file JSON định kỳ để sao lưu.
- Đây là bản MVP; không thay thế ứng dụng native và chưa có tài khoản/cloud sync.


## Nguồn ảnh và video
- Ảnh bài tập tham chiếu từ [Free Exercise DB](https://github.com/yuhonas/free-exercise-db), dữ liệu phát hành theo Unlicense. Ảnh được tải từ GitHub Raw khi thiết bị có kết nối mạng; một số biến thể có thể chưa có ảnh tương ứng và ứng dụng sẽ hiển thị trạng thái thay thế.
- Video không được nhúng sẵn hoặc xác nhận là video cụ thể; nút trong trang chi tiết mở kết quả tìm kiếm YouTube theo đúng tên bài tập để người dùng chọn hướng dẫn phù hợp.
