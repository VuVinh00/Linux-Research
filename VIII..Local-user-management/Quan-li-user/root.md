Trong Linux, tài khoản root là người dùng có quyền lực cao nhất, root có thể làm rất nhiều điều mà ngay cả tài khoản Administrator trên Windows cũng không thể có được.

Trước khi tìm hiểu về user root, chúng ta phân biệt rõ thuật ngữ root trong Linux

Khi đặt vào 3 ngữ cảnh sau, từ root sẽ mang 3 ý nghĩa khác nhau:

- Filesystem: Trong cấu trúc cây thư mục của Linux thì root directory có ký hiệu là dấu **/**, là thư mục cấp cao nhất, nó không có thư mục cha

- Home directory: Mỗi người dùng đều có thư mục chủ ( home ) để lưu trữ những dữ liệu, thiết lập cá nhân của họ. Thư mục home của người dùng root là /root còn những người bình thường khác có thư mục nằm tại /home

- User account: root là tài khoản có đặc quyền cao nhất trong Linux.

**Root** có quyền lực lớn nhất và tuyệt đối, nó có quyền truy cập tới bất kỳ file nào và thực thi được mọi câu lệnh. Ngoài ra, user root có khả năng chỉnh sửa hệ thống rất sâu theo bất kỳ cách nào, ngay cả việc chỉnh sửa các module của hệ điều hành và biên dịch lại Kernel

Nếu đang ở normal user mà muốn chuyển sang user root thì ta sử dụng lệnh:

``$ su root``

Sau đó nhập mật khẩu của user root để đăng nhập với người dùng root
