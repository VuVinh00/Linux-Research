## Thư mục chứa dữ liệu

### /home ( Home Directories )

Là thư mục chính lưu trữ các tập tin cá nhân của tất cả user 

Ví dụ user là vinhvt thì ở thư mục home sẽ có thư mục /home/vinhvt chứa dữ liệu cá nhân của user vinhvt

### /root

Đây là thư mục lưu trữ các tập tin cá nhân của người dùng root

Đây là supper user của hệ thống nên được tách ra với các user còn lại

Chỉ có người dùng root mới có thể truy cập vào thư mục /root

### /srv ( Service Data )

-----------

### /mnt ( Mount Directory )

Chứa các thư mục dùng để admin thực hiện quá trình mount

Vì hệ điều hành Linux coi tất cả là các file và lưu trữ trên 1 cây chung. Đây chính là nơi tạo ra các thư mục để gắn các phân vùng ổ đĩa cứng cũng như các thiết bị khác vào. Sau khi được mount vào đây thì các thiết bị hay ổ cứng sẽ được truy cập như là 1 thư mục.

### /media ( Removeable Media Devices )

Gắn kết các thư mục Temporary ( thư mục tạm thời ) được hệ thống tạo ra khi một thiết bị di động được cắm vào như đĩa CDs, máy ảnh kỹ thuật số, ...

VD: /media/cdrom, /media/floppy ,...

### /tmp ( Temporary Files )

Thư mục chứa các tập tin tạm thời được tạo bởi hệ thống và user

Các tập tin tạo trong thư mục này sẽ được xóa khi hệ thống khởi động lại ( reboot )



