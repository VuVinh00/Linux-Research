## Thư mục tài nguyên hệ thống 

### /usr/bin

/usr/bin là một trong những thư mục chính của /usr, thư mục /usr/bin chứa hầu hết file thực thi ( executable files ), nó không cần dùng để khởi động ( boot ) , hay sửa chữa hệ thống.

Thư mục này chưa hơn 1900 file thực thi trên hệ thống. Một số câu lệnh thông thường được sử dụng đó là awk, bzip2, clear, du, find, free, gunzip, gzip, locate, top, sudo, ....

### /usr/include

Thư mục này bao gồm các header files cho trình biên dịch C. Ví dụ như "stdio.h", "stdlib.h" ,..

Khi bạn nhập thông tin header trong file ngôn ngữ C như #include <stdio.h> thì trình biên dịch sẽ tìm đến file ở /usr/include. Không cần quan tâm đến chúng nếu như bạn không code :D

### /usr/lib 

/usr/lib bao gồm các tệp đối tượng, thư viện và các số nhị phân không được dự định thực thi bởi người dùng hoặc scripts.

### /usr/local

/usr/local là nơi administrator cài đặt phần mềm, phần mềm có thể sử dụng bởi tất cả các user

### /usr/share

Nội dung trong thư mục **/usr/share** chứa các tập tin architecture-independent ( docs, icons, fonts , ... )adm

Hệ thống phân cấp này có thể được chia sẻ với một số hệ điều hành nhất định, tuy nhiên **/usr/share** không được chia sẻ bởi các hệ điều hành khác nhau hoặc các phiên bản khác nhau của 1 hệ điều hành .

Bất kì chương trình hay package nào chứa hoặc yêu cầu dữ liệu không cần sửa đổi thì nên lưu trữ dữ liệu đó trong /usr/share

### /usr/src

**/usr/src** là thư mục con chứa mã nguồn của Kernel, tệp tiêu đề và tài liệu dùng cho mục đích tham khảo 
