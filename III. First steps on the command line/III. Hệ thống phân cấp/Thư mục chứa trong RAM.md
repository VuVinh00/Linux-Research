## Thư mục chứa trong RAM 

### /dev

Chứa các tập tin để nhận biết các thiết bị của hệ thống ( device files ) như các thiết bị đầu cuối, USB hay ổ cứng, các thiết bị được gắn trên hệ thống 

Thư mục này thể hiện một cách rõ ràng là hệ điều hành coi mọi thứ đều là các tệp tin và thư mục, trong thư mục này có thể thấy rất nhiều tập tin đại diện cho các thiết bị như ổ đĩa, cổm COM, ổ CD,... Ta có thể liệt kê bằng lệnh "ls /dev/"

VD:
dev/sda : ổ đĩa thứ nhất

dev/cdrom : ổ CD

### /proc ( Process Information )

Proc là hệ thống file ảo ( pseudo file system ), một hệ thống file thời gian thực ( real time ) và thường trú trong bộ nhớ ( memory resident ) để theo dõi các process đang chạy cùng với trạng thái của hệ thống.

Proc là hệ thống file ảo bởi trên thực tế nó không tồn tại trong bất kì phương tiện lưu trữ nào. Nó tồn tại dựa trên bộ nhớ ảo và dữ liệu luôn thay đổi cùng với trạng thái của hệ thống. Dữ liệu trong /proc luôn được cập nhật liên tục để phù hợp với trạng thái của hệ điều hành.

Nội dung của proc có thể đọc bởi user có quyền thích hợp, trong đó một số phần chỉ có thể đọc bởi owner của process và root.

### /sys

/sys là một giao diện cho kernel, là file hệ thống ảo có thể được dùng truy cập để cài đặt hoặc lấy thông tin về chế độ xem kernel của hệ thống

/sys được dùng từ trước khi Kernel Linux 2.6 được phát hành. Trước đó, tất cả phiên bản Ubuntu đều có /sys
