## Quan hệ 1 - 1  
Quan hệ 1 - 1 là 1 dòng của bảng này liên kết với 1 dòng duy nhất của bảng khác   
***Quan hệ 1 - 1 hình thành do mối liên hệ giữa hai khóa chính của hai bảng***    
Ví dụ:  
- Một công dân chỉ có duy nhất 1 thẻ căn cước công dân và ngược lại, mỗi thẻ căn cước chỉ được cấp cho duy nhất 1 công dân  

- Mỗi một nhân viên chỉ có duy nhất 1 thẻ nhân viên và ngược lại thẻ nhân viên chỉ được cấp cho duy nhất một nhân viên  


![](https://media.techmaster.vn/api/static/bq0a8rs51co78aldi4p0/n0xgbX--)


## Quan hệ 1 - nhiều
Đây là quan hệ rất hay được sử dụng trong thiết kế database. Một dòng của bảng này liên kết với nhiều dòng của bảng khác.  
***Quan hệ 1 - n được hình thành bằng cách tạo liên hệ giữa khóa chính (PRIMARY KEY) và khóa ngoại (FOREIGN KEY)***  

Ví dụ:  
- Một sản phẩm thuộc một danh mục (Thực phẩm, thời trang,...), một danh mục chứa nhiều sản phẩm
- Một nhân viên chỉ thuộc một phòng ban, nhưng một phòng thì lại có nhiều nhân viên  

![](https://media.techmaster.vn/api/static/bq0a8rs51co78aldi4p0/-tqR2JAo)

## Quan hệ nhiều - nhiều
Quan hệ n - n là một dòng của bảng này liên kết tới nhiều dòng của bảng kia và ngược lại 1 dòng ở bảng kia cũng liên kết tới nhiều dòng ở bảng này.  
***Quan hệ n - n được hình thành do mối quan hệ giữa hai khóa ngoại (FOREIGN KEY)***   
Ví dụ:  
- Một sản phẩm có thể nằm trong nhiều đơn hàng, ngược lại một đơn hàng cũng có thể có nhiều sản phẩm
- Một bộ phim có nhiều thể loại, một thể loại cũng có nhiều bộ phim.  
  
  
![](https://media.techmaster.vn/api/static/bq0a8rs51co78aldi4p0/iSWKnjQf)