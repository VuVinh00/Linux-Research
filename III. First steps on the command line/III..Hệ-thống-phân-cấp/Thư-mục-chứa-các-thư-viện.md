## Thư mục chứa các thư viện

### /bin ( user binaries )

Chứa các tập tin thực thi nhị phân ( binary excutables )

Các câu lệnh thường dùng ở chế độ người dùng đơn ( Singer-user mod ) được nằm tại đây

Tất cả user trên hệ thống nằm tại thư mục này đều có thể sử dụng lệnh

VD: ps, ls, ping, grep, cp, ...

### /sbin ( System Binaries )

Cũng giống như /bin, /sbin cũng chứa các tập tin thực thi nhị phân ( binary excutables )

Những câu lệnh này được dùng cho quản trị viên hệ thống và được dùng để bảo trì hệ thống.

VD: iptables, reboot, fdisk, ifconfig, ...

### /lib ( System Libraries )

Chứa các file thư viện hỗ trợ các thư mục nằm dưới /bin và /sbin

Tên file thư viện có thể là id* hoặc lib*.so.*.

Ví dụ: Id-2.1.so, libncurses.so.5.7

### /opt ( Optional add-on Applications )

Chứa các ứng dụng add-on từ nhà cung cấp

Nó chứa các phần mềm và các gói bạn cài đặt mà không cần thiết cho hệ thống cơ sở
