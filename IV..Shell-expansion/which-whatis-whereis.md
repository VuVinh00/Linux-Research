## Chương trình lệnh "which"

Chương trình **which** là một chương trình đơn giản có mục đích xác định đường dẫn các file chương trình thực thi. Nó cho phép người dùng có thể sử dụng output của chương trình làm thông tin đường dẫn tuyệt đối thành input cho các lệnh hay shell script khác

**which** sẽ chỉ tìm đường dẫn các file chương trình nào nằm trong các directory được liệt kê ở biến môi trường **$PATH**. Để xem các directory được liệt kê ở biến môi trường **$PATH** ta dùng lệnh: ``$ echo $PATH``


Cú pháp:

``$ which [-option] [command]``

Ví dụ:

**Hiển thị cơ bản**

```
$ which cat
/bin/cat
```
**Hiển thị toàn bộ đường dẫn của chương trình**

Đối với ví dụ phần 1 thì **which** sẽ mặc định xuất ra thông tin đường dẫn đầu tiên mà chương trình tìm thấy trong các thư mục của biến môi trường **$PATH**. Điều này dẫn đến việc có thể bỏ sót các thông tin đường dẫn khác hay chương trình cùng loại nhưng khác phiên bản trên cùng hệ thống.

Vậy để hiển thị toàn bộ các đường dẫn file chương trình được tìm thấy thì ta thêm option **-a**

```
$ which -a cat
/bin/cat
/usr/bin/cat
```
## Chương trình lệnh whereis

**whereis** là 1 chương trình giúp chúng ta tìm được 3 thông tin sau về 1 chương trình hoặc 1 lệnh trên Linux:

- Đường dẫn vị trí file binary
- Đường dẫn vị trí source code
- Đường dẫn vị trí trang manual dành cho chương trình hay lệnh đó

**whereis** sẽ tìm ở đâu?

Ta có thể dùng câu lệnh **whereis -l** để kiểm tra các đường dẫn mà **whereis** có thể kiểm tra. Như vậy nếu đã cài đặt chương trình ở thư mục khác thì **whereis** sẽ không thể tìm ra được thông tin file chương trình đó.

Cú pháp:

``$ whereis [-option] [command]``

Ví dụ:

```
$ whereis date
date: /bin/date /usr/share/man/man1/date.1.gz
```
