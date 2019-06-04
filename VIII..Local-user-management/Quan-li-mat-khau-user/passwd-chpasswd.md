### Thay đổi password user

#### **passwd**

Mật khẩu của user có thể được set bằng **passwd** và cũng có thể dùng **passwd** để đổi mật khẩu user hiện tại

Cú pháp : 

``passwd + [tên user]``

#### **chpasswd**

**chpasswd** được sử dụng để cập nhật mật khẩu cho user hệ thống Linux khi hoạt động trong chế độ **batch mode** hay còn gọi là tiến trình tự động hóa như shell script.

Chỉ có duy nhất user root hoặc user có cùng quyền hạn mới được phép sử dụng lệnh này.

**chpasswd** hoạt động bằng cách đọc danh sách user và mật khẩu tương ứng từ 1 file text hoặc input trực tiếp prompt. Rồi dùng các thông tin mật khẩu tương ứng đó để thay đổi mật khẩu user

Mặc định mật khẩu có thể cung cấp dưới dạng clear-text và **chpasswd** sẽ tự động mã hóa mật khẩu được cung cấp

- Sử dụng chiều INPUT -STDIN:

Khi gõ lệnh **chpasswd** nó sẽ hiện prompt ra để mình nhập chuỗi dòng kí tự **"user:password"** vào rồi mình phải kết thúc prompt đó

```
# chpasswd
vu:12AAS
vinh:42ddd

(Ctrl+D)
```

Sau khi nhập hết thông tin tên user và mật khẩu sử dụng cho user đó theo format quy định, ấn **Ctrl+D** để xác nhận kết thúc nội dung của input và **chpasswd** sẽ tự động cập nhật mật khẩu mới.

- Sử dụng thông tin từ "pipe": 

Cách này được sử dụng trong shell script cho các hoạt động tự động hóa tác vụ quản trị

``# echo "vuvinh:sfjndsje1234" | chpasswd``

- Đọc nội dung thông tin từ file:

Ta có thể tạo 1 file text chứa thông tin tên user và mật khẩu sử dụng cho user đó làm input đầu vào cho lệnh **chpasswd**. Thông tin user và mật khẩu phải để theo chuẩn format chung :

``<username>:<password>``

Để thực hiện đổi mật khẩu ta chỉ cần chạy lệnh dưới:

``# chpasswd < [đường_dẫn_file]``
