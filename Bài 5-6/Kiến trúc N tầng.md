Kiến trúc 3-tầng được hình thành bằng cách tách ba chức năng chính của ứng dụng thành các tầng (tier) độc lập, thường chạy trên các máy chủ vật lý hoặc logic khác nhau. 

![[3-Tier.png]]

|                                                     |                            |                                                                                                                                                                                 |                                                                             |
| --------------------------------------------------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| Tên lớp (tier)                                      | Vai trò chính              | Nhiệm vụ                                                                                                                                                                        | Ví dụ công nghệ                                                             |
| Trình bày<br><br>(Presentation)                     | Giao diện người dùng       | Xử lý việc hiển thị thông tin, nhận yêu cầu từ người dùng (nhập liệu, bấm chuột) và chuyển tiếp các yêu cầu xuống tầng Logic nghiệp vụ.                                         | Frontend framework (React, Angular, Vue),<br><br>HTML/CSS, Ứng dụng di động |
| Logic nghiệp vụ<br><br>(Business logic/Application) | Logic cốt lõi              | Chứa các quy tắc nghiệp vụ, logic xử lý dữ liệu và điều phối các tác vụ. Đây là “bộ não” của ứng dụng, nơi xử lý các yêu cầu từ tầng Trình bày trước khi tương tác với dữ liệu. | Backend framework (Spring Boot, .NET Core, Node.js/Express), REST APIs      |
| Dữ liệu <br><br>(Data)                              | Lưu trữ và quản lý dữ liệu | Chứa cơ sở dữ liệu (database management system - DBMS), lưu trữ, quản lý, truy xuất và đảm bảo tính toàn vẹn của dữ liệu                                                        | Cơ sở dữ liệu (SQL Server, PostgreSQL, MongoDB), Hệ thống lưu trữ tập tin   |
Ưu điểm:
- Khả năng tái sử dụng: Logic nghiệp vụ nằm ở tầng giữa, độc lập với tầng trình bày. Vì vậy, một logic nghiệp vụ có thể được sử dụng bởi nhiều giao diện khác nhau. Ví dụ: một API xử lý thanh toán có thể được gọi từ cả ứng dụng web và ứng dụng di động
- Khả năng mở rộng: Đây là ưu điểm lớn nhất so với kiến trúc nguyên khối. Bạn có thể mở rộng độc lập theo từng tầng. Ví dụ: thêm máy chủ cho tầng Logic nghiệp vụ khi có nhiều yêu cầu API hơn, mà không cần thêm máy chủ cho tầng Dữ liệu
-  Có tính bảo mật cao: Tầng Dữ liệu được cô lập, chỉ giao tiếp với tầng Logic nghiệp vụ, mà     không giao tiếp với người dùng cuối. Điều này giúp bảo vệ cơ sở dữ liệu khỏi các truy cập trái phép từ bên ngoài
- Dễ phát triển và bảo trì: Vì mỗi tầng có trách nhiệm rõ ràng, các lập trình viên có thể tập trung vào một tầng cụ thể mà không làm ảnh hưởng đến các tầng khác. Đội Frontend có thể làm việc song song với đội Backend, chỉ cần tuân thủ giao diện API

Nhược điểm:
- Phức tạp: Việc thiết lập và quản lý kiến trúc phân tán nhiều tầng phức tạp hơn so với kiến trúc nguyên khối
- Độ trễ: Việc truyền dữ liệu qua nhiều tầng (qua mạng) có thể làm tăng độ trễ (latency) so với việc gọi hàm cục bộ
- Chi phí: Việc duy trì nhiều máy chủ/dịch vụ vật lý hoặc máy ảo cho mỗi tầng sẽ tốn kém hơn

Khi nào thì nên sử dụng kiến trúc 3-tầng:
- Khi ứng dụng của bạn phức tạp, dự kiến phát triển lớn trong tương lai, cần khả năng mở rộng cao và bảo mật dữ liệu được ưu tiên