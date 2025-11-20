Một số đặc điểm:

- Tính độc lập: Mỗi dịch vụ (service) chạy trong tiến trình (process) riêng biệt của nó

- Chức năng chuyên biệt: Mỗi dịch vụ tập trung vào việc thực hiện một chức năng nghiệp vụ cụ thể (ví dụ: dịch vụ quản lý người dùng, dịch vụ xử lý thanh toán, dịch vụ kho hàng)

- Giao tiếp: Các dịch vụ giao tiếp với nhau qua mạng bằng các giao thức nhẹ, phổ biến nhất là RESTful API hoặc message broker (hàng đợi tin nhắn)

- Công nghệ đa dạng (polyglot): Các dịch vụ khác nhau có thể được xây dựng bằng các ngôn ngữ lập trình, framework và thậm chí là cơ sở dữ liệu riêng (independent database) phù hợp nhất với yêu cầu của dịch vụ đó

Mô hình này trái ngược hoàn toàn với kiến trúc nguyên khối (monolithic), nơi mọi thứ được đóng gói thành một đơn vị duy nhất.

![[Microservice-vs-Monolithic.png|500]]

Ưu điểm:

- Khả năng mở rộng độc lập: Có thể mở rộng từng dịch vụ riêng biệt dựa trên nhu cầu tải thực tế, giúp tối ưu hóa tài nguyên (ví dụ: chỉ cần thêm server cho dịch vụ giỏ hàng mà không cần thêm server cho dịch vụ tài khoản)

- Linh hoạt công nghệ: Cho phép các nhóm sử dụng công nghệ (tech stack) tốt nhất cho từng dịch vụ cụ thể (polyglot programming)

- Dễ dàng bảo trì và phát triển: Mã nguồn của mỗi dịch vụ nhỏ và dễ hiểu hơn. Các nhóm phát triển có thể làm việc, triển khai và cập nhật dịch vụ của họ độc lập với các dịch vụ khác (decoupling)

- Khả năng chịu lỗi cao: Nếu một dịch vụ bị lỗi, các dịch vụ khác vẫn có thể tiếp tục hoạt động (fault isolation). Hệ thống không bị sập toàn bộ như trong monolithic

- Triển khai liên tục (CI/CD): Dễ dàng áp dụng DevOps và CI/CD vì chỉ cần triển khai lại các dịch vụ nhỏ đã thay đổi, không cần triển khai toàn bộ ứng dụng lớn

Nhược điểm:

- Phức tạp về vận hành: Việc quản lý, giám sát (monitoring) và gỡ lỗi (debugging) một hệ thống gồm hàng chục hoặc hàng trăm dịch vụ phân tán phức tạp hơn nhiều

- Độ trễ mạng (latency): Các dịch vụ giao tiếp qua mạng (API call) thay vì gọi hàm cục bộ, dẫn đến độ trễ cao hơn so với monolithic

- Quản lý dữ liệu phân tán: Xử lý giao dịch trải dài qua nhiều cơ sở dữ liệu (distributed transactions) rất phức tạp và cần các mẫu thiết kế như Saga

- Chi phí cơ sở hạ tầng: Cần nhiều tài nguyên hơn cho việc chạy nhiều tiến trình, nhiều cơ sở dữ liệu và các công cụ quản lý phức tạp (kubernetes, service mesh, API gateway)

- Kiểm thử tích hợp: Việc đảm bảo tất cả các dịch vụ phối hợp nhịp nhàng với nhau khó khăn hơn so với kiểm thử end-to-end trong monolithic

Khi nào thì nên sử dụng mô hình microservices:

Microservices không phải là giải pháp cho mọi vấn đề. Nó đặc biệt phù hợp khi dự án đạt đến một mức độ phức tạp và quy mô nhất định:

- Hệ thống phức tạp và quy mô lớn: Khi ứng dụng có nhiều chức năng nghiệp vụ riêng biệt và mã nguồn (codebase) trở nên quá cồng kềnh

- Yêu cầu khả năng mở rộng cao và độc lập: Khi một số chức năng (ví dụ: tìm kiếm, streaming) có nhu cầu tải (load) cao hơn nhiều so với các chức năng khác

- Tổ chức lớn với nhiều đội (team autonomy): Khi các nhóm khác nhau có thể sở hữu, phát triển và triển khai dịch vụ của riêng họ mà không bị phụ thuộc vào nhau

- Cần triển khai nhanh chóng và thường xuyên: Khi yêu cầu cập nhật, thêm tính năng mới liên tục và cần thời gian ngưng hệ thống (downtime) tối thiểu

- Có kinh nghiệm vận hành (DevOps maturity): Đội ngũ phát triển đã có kinh nghiệm với các công cụ như Docker, Kubernetes, CI/CD, và các hệ thống giám sát phân tán
