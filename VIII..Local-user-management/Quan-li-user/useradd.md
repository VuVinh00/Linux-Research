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

### Chỉnh sửa thông tin user ( usermod ) 

Sau khi tạo tài khoản, sẽ có lúc cần thay đổi các thuộc tính của user như thư mục lưu trữ của user, tên đăng nhập, login shell, password hết hạn, ... ta có thể sử dụng **usermod**

Khi thực hiện **usermod**, các tệp dưới đây sẽ được sử dụng và tác động

- /etc/passwd - Thông tin tài khoản
- /etc/passwd - Thông tin bảo mật của tài khoản
- /etc/group - Thông tin group
- /etc/gshadow - Thông tin bảo mật của group
- /etc/login.defs

Cú pháp:

``$ usermod [-options] username``

Các tùy chọn (options):

- -c : thay đổi thông tin về username
- -d : thay đổi home directory cho **username**. Thường đi kèm với option **-m** để di chuyển cá file của **username** sang home directory mới
- -e : thay đổi ngày **username** hết hạn
- -f : thay đổi số ngày sau khi password hết hạn cho đến khi **username** bị disable
- -g : thay đổi group chính thức chứa **username**
- -G : thay đổi các group phụ chứa **username**.
- -l : thay đổi tên login của **username**
- -L : khóa **username**
- -p : thay đổi password cho **username**
- -s : thay đổi default shell cho **username**
- -u : thay đổi UID cho **username**
- -U : mở khóa **username**
