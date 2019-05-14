## 1. Đường dẫn tuyệt đối

Đường dẫn tuyệt đối của một tệp tin hay thư mục đều bắt đầu bởi thư mục gốc / (root) và theo cây, theo nhánh, cho đến thư mục hoặc tệp mà bạn mong muốn. Nói đơn giản thì đường dẫn tuyệt đối là đường dẫn bắt đầu bằng / (root)

Ví dụ: Chuyển vào thư mục /home/user

``cd /home/user `` 

Đây là đường dẫn tuyệt đối vì bắt đầu bằng / (root)

## 2. Đường dẫn tương đối

Đường dẫn tương đối thì chúng ta không cần phải bắt đầu từ / (root) mà có thể tiếp cận được với các thư mục hay tập tin bên trong thư mục đang hiện hành (working directory)

Một đường dẫn tương đối thường bắt đầu với:

- Tên của một thư mục hoặc tập tin

- Hệ điều hành dùng ký hiệu "." chỉ thư mục hiện hành và ký hiệu ".." chỉ thư mục mẹ của thư mục hiện hành.

Ví dụ: Bạn đang ở thư mục /home/user mà muốn vào trong thư mục /home/user/download thì chỉ cần nhập:

``cd ../download``


