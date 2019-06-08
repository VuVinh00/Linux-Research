### Standard Input

- Luồng standard input mang dữ liệu từ người dùng đến chương trình. Standard input thường được nhập từ bàn phím 
- Standard input bị kết thúc bởi EOF, EOF có thể được ghi vào bằng Ctrl + D

### Standard Output

- Standard Output in ra những dữ liệu mà được sinh ra bởi chương trình. Khi mà standard output không có điều hướng thì nó sẽ xuất văn bản ra terminal

<img src="https://github.com/vjnkvt/Images/blob/master/output.PNG">

### Standard Error

Standard error viết ra lỗi khi được tạo ra bởi chương trình trong quá trình nó thực thi. Standard error cũng in kết quả ra màn hình

<img src="https://github.com/vjnkvt/Images/blob/master/error.PNG">

### Điều hướng luồng 

Hầu hết kết quả của các command đều được hiển thị ra màn hình. Để chuyển hướng luồng ra đến một file, ta sẽ dùng kí tự **>** như dưới đây :

``# history > history.txt``

Ở ví dụ trên, câu lệnh **history** sẽ được thực thi và kết quả được ghi vào file **history.txt** và kết quả sẽ không được hiển thị ra màn hình 

Kí tự **>>** được dùng để viết tiếp vào file, ví dụ khi dùng **>** nhiều lần thì nội dung sẽ bị ghi đè còn **>>** sẽ viết tiếp vào file đó.
