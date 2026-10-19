# Phối màu cho newsletter

## Mục tiêu

Tạo hai phiên bản newsletter responsive với cùng cấu trúc và nội dung để quan sát tác động của hai nguyên tắc phối màu. Giao diện dùng Bootstrap 5.3.3 qua CDN và CSS variables để quản lý bảng màu.

## Hai phiên bản

- **Phiên bản 1 — Analogous:** xanh lam, xanh biển và xanh ngọc. Các sắc độ gần nhau tạo cảm giác liền mạch, tươi mới và phù hợp với chủ đề sáng tạo, cộng tác.
- **Phiên bản 2 — Complementary:** tím làm màu chủ đạo, vàng cam làm điểm nhấn CTA. Tím gợi cảm giác sáng tạo; vàng cam tạo tương phản thị giác và hướng mắt đến hành động.

Các mã dưới đây là bảng màu đề xuất trong đề bài và được triển khai trực tiếp. Chưa có thao tác tạo/lưu hay xác nhận bảng màu trên Adobe Color.

| Vai trò | Analogous | Complementary |
|---|---|---|
| Primary | `#2563EB` | `#7C3AED` |
| Secondary | `#0EA5E9` | `#A78BFA` |
| Accent | `#14B8A6` | `#F59E0B` |
| Background | `#F8FAFC` | `#FFFBF5` |
| Text | `#1E293B` | `#292524` |
| Card | `#FFFFFF` | `#FFFFFF` |

Giao diện có thêm các sắc chuyển nhẹ, màu chữ phụ và màu chữ CTA để tạo chiều sâu và tăng độ dễ đọc. Màu phụ và điểm nhấn được khai báo trong CSS variables; nền CTA ở phiên bản 2 là tím nhạt để chữ và nút vàng cam nổi rõ.

## Chạy project

1. Mở thư mục `newsletter-project` trong VS Code.
2. Cài extension **Live Server** nếu máy chưa có.
3. Mở `index.html`, chọn **Go Live** để xem trang chọn phiên bản.
4. Có thể mở trực tiếp `newsletter-version-1.html` hoặc `newsletter-version-2.html`; cả hai trang hoạt động độc lập với đường dẫn CSS tương đối.

Bootstrap được tải từ jsDelivr, vì vậy cần kết nối Internet để nạp stylesheet của Bootstrap. Phần bố cục, màu sắc và tương tác cơ bản còn lại nằm trong các file dự án.

## So sánh cảm nhận thị giác

Analogous dùng các màu lạnh nằm gần nhau nên giao diện êm, thống nhất và thoáng. Complementary tạo nhịp mạnh hơn: nền ngà và tông tím cho cảm giác ấm, có cá tính; nút vàng cam trở thành điểm dừng thị giác rõ ràng. Nội dung, kích thước card và cấu trúc được giữ tương đương để việc so sánh tập trung vào màu sắc.

## Đối chiếu trên Adobe Color và ảnh minh chứng

1. Mở [Adobe Color](https://color.adobe.com/create/color-wheel) trong trình duyệt.
2. Chọn quy tắc **Analogous**, nhập/chọn màu xanh lam làm màu gốc, rồi đối chiếu các màu lân cận với `#2563EB`, `#0EA5E9`, `#14B8A6`.
3. Chọn quy tắc **Complementary**, nhập/chọn tím `#7C3AED` làm màu gốc; xem màu đối diện và so sánh với điểm nhấn cam `#F59E0B`. Bộ màu đề xuất có màu phụ `#A78BFA` để hỗ trợ sắc tím.
4. Ghi lại mã HEX Adobe Color thực tế hiển thị. Nếu khác các mã đề xuất ở trên, cập nhật README/CSS theo kết quả bạn chọn.
5. Chụp ảnh màn hình từng quy tắc sao cho thấy tên quy tắc, bánh xe màu và các mã HEX; lưu vào project nếu cần nộp minh chứng. Chỉ ghi rằng đã tạo/lưu trên Adobe Color sau khi hoàn thành thao tác đó.

## Khả năng đọc và responsive

Nền sáng, card trắng, chữ đậm và vùng nội dung giới hạn chiều rộng giúp dễ đọc. CTA ở bản 2 dùng chữ tối trên vàng cam; các liên kết có trạng thái hover và mọi nút/liên kết có viền focus nhìn thấy được khi dùng bàn phím. Bootstrap xếp hai card cạnh nhau từ màn hình cỡ tablet trở lên và xếp dọc trên điện thoại. Các nút CTA mở email soạn sẵn; liên kết bài viết cuộn tới khu vực hành động trong trang.
