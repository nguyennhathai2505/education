# Website Demo Bản Việt — Bản Xuất HTML Tĩnh

Bản tĩnh chụp từ website fullstack "Website Bản Việt" (sau khi đã sửa bố cục website chuẩn và sửa màu theo logo gốc), dùng để xem offline, gửi đối tác hoặc bàn giao đội dev làm tham chiếu front-end.

## Cấu trúc folder

- `index.html` — file HTML full của toàn bộ website (9 khu vực, điều hướng bằng hash routing: Trang chủ, Giới thiệu, Hệ sinh thái, 4 trang thương hiệu Điểm 10+ / DanhLingo / Aitechco / Schooli, Khóa học + chi tiết, Tin tức + bài viết, Liên hệ, Quản trị demo).
- `assets/` — 13 file hình: 8 ảnh lớp học + 5 logo thật (logo-banviet.png, logo-diem10.png, logo-danhlingo.png, logo-aitechco.png, logo-schooli.png).
- Ngoài ra còn có bản 1 file duy nhất `website-banviet-full-1-file.html` (toàn bộ hình đã nhúng sẵn vào HTML) — mở trực tiếp là chạy, không cần thư mục assets.

## Cách mở

Mở `index.html` bằng trình duyệt (Chrome/Edge). Muốn giống chạy thật, có thể đưa cả folder lên bất kỳ hosting tĩnh nào (WordPress hosting, Netlify, Vercel, GitHub Pages...) — không cần cài đặt thêm.

## Lưu ý quan trọng cho đội dev

- Đây là bản TĨNH để trình diễn giao diện: form đăng ký tư vấn lưu vào **localStorage** của trình duyệt, trang Quản trị đọc từ đó. Khi triển khai thật phải nối backend (lưu đăng ký vào cơ sở dữ liệu + gửi thông báo cho bộ phận tư vấn).
- Màu thương hiệu theo logo gốc đã kiểm chứng: Bản Việt navy #0B2C5C / #07204A, blue #1565D8; Điểm 10+ đỏ #E2231A + gold #F2C200; DanhLingo đỏ #D61F26 + vàng #FCB900; Aitechco xanh #32BAEC + cam #FBAF17; Schooli navy #004080 → teal #00A2D4 (accent #0B6FA4). Font: Be Vietnam Pro (tải từ Google Fonts, cần internet; offline sẽ fallback sans-serif).
- Logo trong assets là bản PNG raster — trước khi chạy production nên xin file vector (AI/SVG) chính thức của 4 thương hiệu.
- Số liệu trên trang chỉ dùng số đã kiểm chứng (từ 2010, 4 thương hiệu, 8 cơ sở Điểm 10+ tại TP.HCM, 100% giáo viên Anh ngữ chuẩn quốc tế). Không tự thêm số học viên / tỉ lệ đỗ khi chưa có xác thực từ Bản Việt.
