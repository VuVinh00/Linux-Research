## Filesystem là gì ?
Filesystem là thứ xác định các thức tổ chức, quản lý dữ liệu hay có thể nói là quản lý cách thức dữ liệu được đọc và lưu trên thiết bị. Filesystem cho phép người dùng truy cập nhanh chóng và an toàn khi vào các tệp tin thư mục khi cần thiết.

Những loại Filesystem được hỗ trợ trên Linux:
- Filesystem cơ bản : ext2, ext3, ext4, XFS, Btrfs, JFS, NTFS, ...
- Filesystem dành cho dạng lưu trữ Flash ( thẻ nhớ, ...): ubifs, JFFS2, YAFFS, ...
...

## Cấu trúc Filesystem trên Linux

Filesystem trên Linux lưu trữ những file quan trọng theo một tiêu chuẩn được gọi là FHS ( Filesystem Hierarchy Standard ). Trong FHS, tất cả file và thư mục đều nằm trong thư mục root **/**. Việc có một tiêu chuẩn như này giúp người dùng, quản trị viên, lập trình viên có thể chuyển đổi giữa các Distro một cách dễ dàng

<img src="https://github.com/vinhvt2704/Images/blob/master/filesystem.png">

Chức năng của từng thư mục trong Linux:

**/bin**: Các chương trình cơ bản

**/boot**: Chứa Linux Kernel

**/dev**: Chứa các tập tin thiết bị ( CDRom, HDD, SSD,...)

**/etc**: Chứa các tập tin cấu hình hệ thống

**/home**: Thư mục dành cho user

**/lib**: Chứa các thư viện dùng chung cho các tập lệnh nằm trong /bin và /sbin. Thư mục này cũng chưa các module của kernel 

**/mnt** hoặc **/media**
Mount point cho những hệ thống file kết nối tới bên ngoài

**/opt**: Thư mục chưa các phần mềm cài thêm

**/sbin**: Các chương trình của hê thống

**/srv**: Dữ liệu được sử dụng bởi các máy chủ lưu trữ trên hệ thống

**/tmp**: Thư mục chứa các file tạm thời

**/usr**: Thư mục chứa những file cố định hoặc quan trọng để phục vụ tất cả người dùng

**/var**: Dữ liệu biến được xử lí bở daemon. Bao gồm các tệp nhật ký, hàng đợi, bộ đệm, cache

**/root**: Tệp cá nhân của người dùng root

**/proc**: Là một hệ thống file ảo, một hệ thống file thời gian thực và thường trú trong bộ nhớ để theo dõi các process đang chạy cùng với trạng thái của hệ thống
