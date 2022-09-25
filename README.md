## Database
Database - Cơ sở dữ liệu là một tập hợp các dữ liệu có tổ chức liên quan đến nhau, thường được lưu trữ và truy cập điện tử từ hệ thống máy tính. Khi cơ sở dữ liệu phức tạp hơn, chúng thường được phát triển bằng cách sử dụng các kỹ thuật thiết kế và mô hình hóa chính thức (Wikipedia).  

Database hỗ trợ 2 chức năng chính: 
- Lưu trữ dữ liệu  
- Thao tác với dữ liệu  

Các thao tác với dữ liệu gồm:  
- Đọc dữ liệu từ database  
- Thêm dữ liệu mới
- Chỉnh sửa dữ liệu sẵn có  
- Xóa dữ liệu  
- Backup và khôi phục dữ liệu  

## Phân loại database  
Có nhiều cách khác nhau để phân loại database, ở đây mình sẽ chia ra thành 2 loại:  

### Cơ sở dữ liệu quan hệ
Cơ sở dữ liệu quan hệ tổ chức dữ liệu theo các bảng và các bảng có quan hệ với nhau để giảm thiểu sự dư thừa dữ liệu đồng thời vẫn đảm bảo sự hiệu quả trong lưu trữ và truy xuất dữ liệu

**Các thành phần cơ bản của một số cơ sở dữ liệu quan hệ:**  
- Bảng dữ liệu (Table)  
- Mối quan hệ (Relation)  
- Lược đồ thực thể (ERD - Entity Relationship Diagram)  

Một số CSDL quan hệ phổ biến như: Oracle, MySQL, PostgreSQL, SQL Server,...  

### Cơ sở dữ liệu phi quan hệ (NoSQL)
NoSQL lưu trữ dữ liệu của mình theo dạng cặp giá trị `key-value`. Sử dụng số lượng lớn các node để lưu trữ thông tin. Nó lưu trữ và quản trị dữ liệu sao cho có thể hỗ trợ được tốc độ vận hành ở công xuất cao và cung cấp tính linh hoạt tuyệt vời cho các nhà phát triển khi sử dụng.  
Một số NoSQL phổ biến: MongDB, Cassandra, HBase,...  
Tuy nhiên, hệ thống NoSQL không nhất quán dữ liệu giống như SQL. Trên thực tế, cơ sở dữ liệu SQL không ưu tiên hiệu xuất và khả năng mở rộng mà thường sẽ đẩy việc tuân thủ các thuộc tính ACID đảm bảo độ tin cậy cho các giao dịch lên trước, trong khi CSDL NoSQL gần như bỏ qua các đảm bảo ACID để ưu tiên tốc độ và khả năng mở rộng  

## MySQL
MySQl là một hệ thống quản trị cơ sở dữ liệu mã nguồn mở (RDBMS - Relational Database Management System) hoạt động theo mô hình client-server. MySQL được tích hợp Apache, PHP. MySQL quản lý dữ liệu thông qua các cơ sở dữ liệu. Mỗi cơ sở dữ liệu có thể có nhiều bảng quan hệ chứa dữ liệu. MySQL cũng có cách truy vấn và mã lệnh tương tự với SQL.  


![mysql-logo](https://media.techmaster.vn/api/static/bq0a8rs51co78aldi4p0/NCgwtBEQ)

Các bạn có thể xem source code của nó tại: [https://github.com/mysql/mysql-server](https://github.com/mysql/mysql-server)  

MySQL được sử dụng bởi rất nhiều công ty lớn, nổi tiếng trên thế giới: Youtube, Spotify, Netflix, Facebook, NASA, Pinterest,...    

## MySQL Workbench

MySQL Workbench là một công cụ thiết kế cơ sở dữ liệu trực quan thống nhất hoặc công cụ giao diện, đồ họa được sử dụng để làm việc bởi kiến trúc sư cơ sở dữ liệu, nhà phát triển và quản trị viên cơ sở dữ liệu. Nó được phát triển và duy trì bởi Oracle.   

MySQL Workbench cung cấp phát triển SQL, mô hình hóa dữ liệu, di chuyển dữ liệu và các công cụ quản trị toàn diện để cấu hình server, quản trị người dùng, sao lưu và nhiều chức năng khác. Chúng ta có thể sử dụng Server Administration để tạo mô hình dữ liệu vật lý mới, sơ đồ E-R và để phát triển SQL (chạy truy vấn,…). Nó có sẵn cho tất cả các hệ điều hành chính như Mac OS, Windows, Ubuntu và Linux. MySQL Workbench hỗ trợ đầy đủ MySQL Server cho phiên bản v5.6 trở lên. 