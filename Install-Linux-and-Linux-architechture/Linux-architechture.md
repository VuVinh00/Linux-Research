## Kiến trúc hệ điều hành Linux

Hệ thống Linux hoạt động cơ bản ở 4 layer. Nhìn vào sơ đồ bên dưới ta có thể thấy kiến trúc của hệ điều hành Linux

<img src="https://github.com/vjnkvt/Images/blob/master/linux-architecture-image.png">

- **Hardware**( phần cứng ): Phần cứng bao gồm tất cả thiết bị vật lý được gắn vào hệ thống. Ví dụ như: Hard disk drive, RAM, CPU, ...

- **Kernel** ( nhân ): Kernel là trung tâm điều khiển của hệ điều hành Linux, chứa các mã nguồn điều khiển hoạt động của toàn bộ hệ thống, tương tác trực tiếp với phần cứng

- **Shell**: Shell là giao diện để người dùng thao tác với kernel.

  * Bash shell là shell mặc định trên Linux được viết bởi Brian Fox và Chet Ramey cho dự án GNU. Bash được cải tiến từ sh, hỗ trợ nhiều câu lệnh hơn

- **Applications**: Đây là các chương trình tiện ích được chạy trên Shell. Nó có thể là nhiều ứng dụng như: Web brower, media player, ...
