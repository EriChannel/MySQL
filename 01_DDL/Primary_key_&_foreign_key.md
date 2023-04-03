## PRIMARY KEY
PRIMARY KEY là một ràng buộc (constraint) áp dụng cho một hoặc nhiều cột.  
Khi được gắn PRIMARY KEY, giá trị của (các) cột đó sẽ là độc nhất (unique) và không có giá trị null  
- Độc nhất (unique): Không có các giá trị trùng nhau  
- Không có giá trị null: Nếu chúng ta INSERT hoặc UPDATE cột PRIMARY KEY với giá trị null thì database sẽ thông báo lỗi  

Mỗi bảng chỉ có tối đa một PRIMARY KEY    

### Tác dụng của PRIMARY KEY  
Có thể hình dùng PRIMARY KEY giống như số thẻ căn cước, mã nhân viên hay mã học sinh của bạn: Khi biết được một giá trị thì sẽ tìm ra được tất cả các thông tin còn lại của đối tượng đó.  

### Tạo PRIMARY KEY  
Vẫn với bảng `readers`, lúc này mình sẽ sử dụng `id` để làm PRIMARY KEY    
```sql
CREATE TABLE readers (
    id INT PRIMARY KEY,
    name TEXT,
    date_of_birth DATE,
    address TEXT,
    mobile TEXT,
    email TEXT
)
```

## FOREIGN KEY  
FOREIGN KEY cũng là một ràng buộc được áp dụng cho một hoặc nhiều cột. Khi một cột được gắn ràng buộc FOREIGN KEY thì giá trị của cột đó sẽ nối đến một PRIMARY KEY trong bảng khác  

### Tác dụng của FOREIGN KEY  
FOREIGN KEY dùng để kết nối dữ liệu của 2 bảng với nhau  
Ví dụ chúng ta có hai bảng `employee` và `department`  

| Tên cột | Kiểu dữ liệu |
| --- | --- |
| id | int |
| name | text |  
 
<br>

| Tên cột | Kiểu dữ liệu |
| --- | --- |
| id | int |
| full_name | text |
| birthday | date |
| gender | enum ("male", "female") |
| address | text |
| mobile | varchar(15) |
| id_departmant | int |

**Câu lệnh tạo bảng:**  

- Tạo bảng `department`  
```sql
CREATE TABLE department(
    id INT PRIMARY KEY,
    name text
)
```

- Tạo bảng `employee`
```sql
CREATE TABLE employee(){
    id INT PRIMARY KEY,
    full_name text,
    birthday DATE,
    gender enum("male", "female"),
    address text,
    mobile varchar(15),
    id_department int,
    FOREIGN KEY (id_department) REFERENCES department(id)
}
