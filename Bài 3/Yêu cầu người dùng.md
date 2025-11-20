
Yêu cầu người dùng (user requirement) là những nhu cầu, mong đợi, và kỳ vọng của người dùng cuối về một sản phẩm, hệ thống, hoặc dịch vụ. Nó mô tả những gì người dùng mong đợi hệ thống thực hiện để giải quyết vấn đề của họ.

Yêu cầu người dùng chia thành 2 loại: chức năng (tính năng của hệ thống) và phi chức năng (tốc độ, hiệu suất, tin cậy).

Yêu cầu được viết bằng ngôn ngữ tự nhiên, dễ hiểu, không mang tính kỹ thuật. Yêu cầu người dùng thường được thu thập thông qua phỏng vấn, khảo sát, và các buổi họp với khách hàng hoặc người dùng cuối.

Yêu cầu này thường được ghi lại trong một tài liệu gọi là [Tài liệu đặc tả yêu cầu người dùng](https://www.google.com/search?cs=0&sca_esv=518de7ca735d1bf8&q=T%C3%A0i+li%E1%BB%87u+%C4%91%E1%BA%B7c+t%E1%BA%A3+y%C3%AAu+c%E1%BA%A7u+ng%C6%B0%E1%BB%9Di+d%C3%B9ng&sa=X&ved=2ahUKEwiozcbigb6PAxVQoa8BHXM7EcEQxccNegQIBRAB&mstk=AUtExfBi2lqwSs0FaQ-OCrHrJVrN4GgUqkrszafRA_ah0AYDNiiAM8ypyyDaDZRr2UwWiyVhIuD0-IgMPowbxKMZCBgnHznj8gUJ0PFFigeiHEWmiHoi48mkLJghor3iU7l2XhndIXJYv9meuGu9Z77Dkf2QJNhwD-hZ2KWRo8jlcXtm0p8&csui=3) (User Requirement Specification - URS) để làm cơ sở cho việc thiết kế và phát triển sản phẩm. 

Mục đích của yêu cầu người dùng

- Định hướng phát triển: Giúp đội ngũ phát triển và kỹ sư hiểu rõ nhu cầu của người dùng để xây dựng sản phẩm đúng mong muốn.

- Đảm bảo sự hài lòng: Sản phẩm cuối cùng sẽ đáp ứng các kỳ vọng của người dùng, mang lại trải nghiệm tốt và sự hài lòng.

- Quản lý dự án: Là cơ sở để lập kế hoạch, ước tính chi phí, kiểm soát dự án và đánh giá thành công. 

Đặc điểm của yêu cầu người dùng

- Từ góc độ người dùng: Tài liệu URS được viết theo góc nhìn của người dùng cuối, không quá kỹ thuật hay phức tạp, và để người dùng có kiến thức chung về hệ thống có thể hiểu được. 

- Chức năng và phi chức năng: Bao gồm các tính năng mà hệ thống cần có (chức năng) và các yếu tố khác như hiệu suất, tốc độ, độ tin cậy (phi chức năng).

- Làm cơ sở cho tài liệu kỹ thuật: Là nền tảng cho các tài liệu đặc tả kỹ thuật do đội ngũ phát triển tạo ra, quy định cách thức đáp ứng yêu cầu của người dùng.

## Yêu cầu chức năng

Yêu cầu chức năng là các tính năng cụ thể mà một hệ thống phải thực hiện để đáp ứng nhu cầu của người dùng.

Ví dụ, yêu cầu tính năng của hệ thống Bán sách trực tuyến, gồm:

1. Yêu cầu liên quan đến người dùng

Các yêu cầu này tập trung vào việc quản lý thông tin và tương tác của người dùng với hệ thống.

(FR là viết tắt của Functional Requirements: yêu cầu chức năng)

- Đăng ký và đăng nhập:

+ FR-1.1: Hệ thống phải cho phép người dùng mới đăng ký tài khoản bằng cách cung cấp email, tên đầy đủ và mật khẩu.

+ FR-1.2: Hệ thống phải xác thực thông tin đăng nhập của người dùng đã có tài khoản.

+ FR-1.3: Hệ thống phải cung cấp tính năng "Quên mật khẩu", cho phép người dùng đặt lại mật khẩu qua email.

- Quản lý tài khoản cá nhân:

+ FR-1.4: Người dùng phải có khả năng cập nhật thông tin cá nhân của họ, bao gồm tên, địa chỉ, số điện thoại.

+ FR-1.5: Người dùng phải có thể xem lịch sử mua hàng của họ, bao gồm các đơn hàng đã đặt, trạng thái đơn hàng và chi tiết các sản phẩm đã mua.

2. Yêu cầu liên quan đến sản phẩm và tìm kiếm

Những yêu cầu này mô tả cách người dùng tương tác với danh mục sản phẩm.

- Tìm kiếm và lọc sản phẩm:

+ FR-2.1: Hệ thống phải cho phép người dùng tìm kiếm sách theo tiêu đề, tác giả, hoặc nhà xuất bản.

+ FR-2.2: Người dùng phải có khả năng lọc kết quả tìm kiếm theo nhiều tiêu chí như thể loại (tiểu thuyết, kinh tế, khoa học), giá cả, hoặc đánh giá của người dùng.

- Hiển thị thông tin sản phẩm:

+ FR-2.3: Hệ thống phải hiển thị một trang chi tiết cho mỗi cuốn sách, bao gồm hình ảnh bìa, mô tả, giá, tác giả, và các thông số kỹ thuật khác (số trang, năm xuất bản).

+ FR-2.4: Trang chi tiết sản phẩm phải hiển thị các đánh giá và nhận xét từ những người dùng khác.

3. Yêu cầu liên quan đến giỏ hàng và thanh toán

Các yêu cầu này mô tả quy trình mua hàng, từ khi thêm sản phẩm vào giỏ đến khi hoàn tất thanh toán.

- Quản lý giỏ hàng:

+ FR-3.1: Người dùng phải có khả năng thêm một hoặc nhiều cuốn sách vào giỏ hàng.

+ FR-3.2: Người dùng có thể chỉnh sửa số lượng sách trong giỏ hàng hoặc xóa sách ra khỏi giỏ.

+ FR-3.3: Giỏ hàng phải tự động cập nhật tổng giá trị đơn hàng khi có thay đổi về số lượng hoặc sản phẩm.

- Thanh toán và đặt hàng:

+ FR-3.4: Hệ thống phải cho phép người dùng lựa chọn phương thức thanh toán.

+ FR-3.5: Hệ thống phải gửi một email xác nhận đơn hàng tới người dùng sau khi thanh toán thành công, kèm theo chi tiết đơn hàng và mã theo dõi.

4. Yêu cầu liên quan đến đánh giá và nhận xét

- FR-4.1: Người dùng đã mua một cuốn sách phải có khả năng viết đánh giá và xếp hạng (ví dụ, từ 1 đến 5 sao) cho cuốn sách đó.

- FR-4.2: Các đánh giá phải được hiển thị trên trang chi tiết sản phẩm và được sắp xếp theo thời gian hoặc độ hữu ích.

## Yêu cầu phi chức năng

Yêu cầu phi chức năng không tập trung vào các tính năng cụ thể, mà quan tâm tới chất lượng của hệ thống, như tốc độ, bảo mật, khả năng mở rộng, độ tin cậy.

Ví dụ:

Các yêu cầu phi chức năng của hệ thống Bán sách trực tuyến:

1. Hiệu suất (Performance)

- Tốc độ tải trang: Trang chủ và trang danh sách sản phẩm phải tải hoàn toàn trong vòng dưới 3 giây, ngay cả trong giờ cao điểm.

- Thời gian phản hồi: Hệ thống phải xử lý yêu cầu tìm kiếm và lọc sản phẩm trong vòng chưa đầy 2 giây.

- Khả năng chịu tải: Hệ thống phải có khả năng xử lý đồng thời 5.000 người dùng mà không bị chậm hoặc ngừng hoạt động.

2. Khả năng sử dụng (Usability)

- Giao diện trực quan: Giao diện người dùng phải dễ hiểu, các nút và liên kết phải rõ ràng để người dùng có thể dễ dàng tìm kiếm, thêm sách vào giỏ hàng và thanh toán mà không cần hướng dẫn.

- Tương thích đa nền tảng: Website phải hiển thị và hoạt động tốt trên các trình duyệt phổ biến như Chrome, Firefox và trên các thiết bị di động (điện thoại, máy tính bảng) với các kích thước màn hình khác nhau.

- Trợ giúp và hỗ trợ: Hệ thống nên có các mục FAQ (câu hỏi thường gặp) hoặc chatbot để trả lời các câu hỏi cơ bản của người dùng.

3. Bảo mật (Security)

- Bảo vệ dữ liệu người dùng: Tất cả thông tin cá nhân của người dùng, bao gồm tên, địa chỉ, và mật khẩu, phải được mã hóa và lưu trữ an toàn.

- Bảo mật thanh toán: Toàn bộ giao dịch thanh toán phải tuân thủ các tiêu chuẩn bảo mật quốc tế (ví dụ: PCI DSS) để đảm bảo thông tin thẻ tín dụng của người dùng được bảo vệ.

- Chống tấn công: Hệ thống phải có cơ chế bảo vệ chống lại các cuộc tấn công mạng phổ biến như SQL Injection và XSS (Cross-Site Scripting).

4. Độ tin cậy (Reliability)

- Thời gian hoạt động (Uptime): Hệ thống phải đảm bảo thời gian hoạt động ít nhất 99.9% mỗi tháng, tức là không được ngừng hoạt động quá 44 phút.

- Sao lưu dữ liệu: Dữ liệu người dùng và đơn hàng phải được sao lưu tự động hàng ngày để có thể khôi phục lại trong trường hợp xảy ra sự cố.

5. Khả năng mở rộng (Scalability)

- Mở rộng kho sách: Hệ thống phải được thiết kế để dễ dàng thêm hàng nghìn đầu sách mới mà không ảnh hưởng đến hiệu suất.

- Hỗ trợ tính năng mới: Kiến trúc hệ thống phải cho phép tích hợp các tính năng bổ sung trong tương lai, chẳng hạn như hệ thống tích điểm thưởng cho khách hàng hoặc chương trình giới thiệu sản phẩm.