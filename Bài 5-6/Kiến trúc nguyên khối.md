## Kiến trúc nguyên khối
![[KienTrucNguyenKhoi.png|500]]
Trong đó:
- Giao diện người dùng (user interface)
- Logic nghiệp vụ (business layer)
- Truy cập dữ liệu (data interface)

![[Monolith-Example.png]]
Ưu điểm:
- Quá trình phát triển, triển khai đơn giản: Do tất cả nằm trong một khối duy nhất, việc phát triển, thử nghiệm và triển khai sẽ đơn giản hơn.
- Hiệu suất cao: Do không có giao tiếp liên bộ phận, ứng dụng thường có hiệu suất cao hơn.
Nhược điểm:
- Khó bảo trì và mở rộng: Khi ứng dụng phát triển lớn hơn, việc bảo trì và thêm tính năng mới trở nên phức tạp
- Khả năng chịu lỗi kém: Một lỗi nhỏ có thể làm gián đoạn toàn bộ hệ thống

Khi nào thì nên sử dụng mô hình nguyên khối:
- Dự án nhỏ, cần triển khai nhanh
- Đội ngũ phát triển ít thành viên
- Tài nguyên, máy móc ít
- Việc giao tiếp giữa các thành phần của ứng dụng cần hiệu suất cao

Ví dụ về các ứng dụng theo kiến trúc nguyên khối:
- Hầu hết các ứng dụng desktop truyền thống đều được thiết kế theo kiểu kiến trúc nguyên khối. Kiến trúc nguyên khối rất phù hợp với môi trường desktop vì toàn bộ ứng dụng chạy cục bộ trên một máy tính duy nhất.
- Hệ quản trị nội dung (CMS) cũ (wordpress), ứng dụng thương mại điện tử nhỏ