## Chương trình lệnh "which"

Chương trình **which** là một chương trình đơn giản có mục đích xác định đường dẫn các file chương trình thực thi. Nó cho phép người dùng có thể sử dụng output của chương trình làm thông tin đường dẫn tuyệt đối thành input cho các lệnh hay shell script khác

**which** sẽ chỉ tìm đường dẫn các file chương trình nào nằm trong các directory được liệt kê ở biến môi trường **$PATH**. Để xem các directory được liệt kê ở biến môi trường **$PATH** ta dùng lệnh: ``$ echo $PATH``


Cú pháp:

``$ which [-option] [command]``

Ví dụ:

**Hiển thị cơ bản**

```$ which cat
/bin/cat
```
