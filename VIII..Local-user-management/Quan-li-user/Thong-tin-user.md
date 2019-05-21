## Thông tin của user

Thông tin của user trong Linux sẽ được lưu trữ trong file **/etc/passwd**. Ta có thể dùng lệnh **cat** để đọc file /etc/passwd.

<img src="https://github.com/vinhvt2704/Images/blob/master/passwd.PNG">

Giải thích:

**vuvinh** ( username ): tên đăng nhập

**x** ( password ): nếu có sử dụng /etc/shadow thì ở đây sẽ là chữ x (/etc/shadow chứa mật khẩu được hash

**1000:1000** ( user ID : group ID): user ID để phân biệt người này với người khác

**vuVinh** ( comments ): mô tả cho user

**/home/vuvinh** ( HomeDirectory ): thư mục home của từng user

**/bin/bash** ( Shell ): Tên chương trình sẽ được thực thi ngay sau khi user login vào. Nếu không có shell user sẽ không thể login
