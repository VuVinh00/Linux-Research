## Thông tin cơ bản của hệ thống

### File /proc/bus

**/proc/bus** là thư mục chứa thông tin về các giao tiếp trong hệ thống. Các thư mục con và các file trong /proc/bus có thể khác nhau dựa vào các thiết bị kết nối trên hệ thống.

### lsusb

Câu lệnh **lsusb** giúp hiển thị thông tin về các USB đang chạy trên hệ thống và các thiết bị được kết nối với chúng.

Để chạy lệnh **lsusb** bạn có thể nhập **lsusb** từ chính màn hình dòng lệnh ( terminal)

``$ lsusb``

<img src="https://github.com/vinhvt2704/Images/blob/master/lsusb.PNG">

**lsusb** sẽ đưa ra cho bạn các drivers và thiết bị được kết nối trên hệ thống

Cách đọc kết quả, ví dụ

**Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub**
- **Bus 001**: nghĩa là nơi thiết bị được gắn kết
- **Device 001**: nghĩa là thiết bị thứ nhất được gắn kết
- **ID**: Nghĩa là số ID của thiết bị
- **Linux Foundation 2.0 root hub**: Tên drivers 

### File /proc/interrupts

Ta có thể liệt kê danh sách gián đoạn bằng cách dùng lệnh cat đọc file **/proc/interrupts**

<img src="https://github.com/vinhvt2704/Images/blob/master/interrupts.PNG">

### lscpu

Câu lệnh **lspcu** dùng để hiển thị thông tin về kiến trúc của CPU. 

Cú pháp:

``$ lscpu``

<img src="https://github.com/vinhvt2704/Images/blob/master/lscpu.PNG">

### lsblk

**lsblk** được dùng để hiển thị thông tin các thiết bị lưu trữ như ổ cứng, ổ flash(usb)

<img src="https://github.com/vinhvt2704/Images/blob/master/lslbk.PNG">

### Cách kiểm tra distro, phiên bản Linux đang dùng

Ta có thể dùng câu lệnh ``cat /etc/*-release`` để kiểm tra bản phân phối đang dùng

<img src="https://github.com/vinhvt2704/Images/blob/master/checkdistro.PNG">
