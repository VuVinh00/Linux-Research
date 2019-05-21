### Tạo user mới useradd

**useradd** dùng để tạo ra user mới

Cú pháp:

``$ useradd [-option] [tên-user]``

Khi câu lệnh useradd được tạo, nó sẽ lấy một số thông tin từ trong /etc/default/useradd. Ta có thể kiểm tra thuộc tính của /etc/default/useradd bằng câu lệnh **vi**

<img src="https://github.com/vinhvt2704/Images/blob/master/default.PNG">

Giải thích:

**GROUP**: Số group tối đa mà user có thể là member

**HOME**: Nơi thư mục của user khi user mới được tạo

**INACTIVE**: Số ngày hết hạn của tài khoản ( INACTIVE=-1 nghĩa là luôn hoạt động )

**EXPRIRE**: Ngày tài khoản hết hạn

**SHELL**: login shell mặc định cho user

**SKEL**: Nơi mà các tệp hồ sơ người dùng mặc định được sao chép vào thư mục chính của người 
dùng

**CREATE_MAIL_SPOOL**: Tùy chọn này sẽ tạo một thư mục của người dùng trong /var/main, nơi có thể lưu trữ mail.

Bằng cách sửa file /etc/default/useradd, ta có thể thay đổi shell mặc định và thư mục chứa user 

### Xóa user đang tồn tài ( userdel )

**userdel** dùng để xóa tài khoản người dùng và các tệp có liên quan

``$ userdel [-option] LOGIN``

Ví dụ:

``$ userdel vuvinh``
