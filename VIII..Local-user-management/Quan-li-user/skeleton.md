### Tìm hiểu /etc/skel

Thư mục /etc/skel được sử dụng để tạo home directory khi có user mới được tạo. Các file trong /etc/skel có thể như bên dưới:

<img src="https://github.com/vinhvt2704/Images/blob/master/skel.PNG">

( /etc/skel được định nghĩa trong /etc/default/useradd, ta có thể thay đổi đường dẫn mặc định /etc/skel tới các địa điểm khác )

**Quyền hạn mặc định của /etc/skel**
- Mặc dịnh thì quyền hạn của /etc/skel là drwxr-xr-x
- Không nên thay đổi quyền hạn của thư mục skel hoặc nội dung của nó. Thay đổi quyền hạn có thể phá hủy 1 số chương trình, bởi trong thư mục skel có một số cấu hình cần cho phép đọc
