## Cách sử dụng biến trong Shell

**Biến** là một chuỗi kí tự mà chúng ta có thể gán giá trị cho chúng. Giá trị được gán có thể là một số, văn bản, hoặc bất kỳ kiểu dữ liệu nào và xóa chúng

### Quy tắc đặt tên biến trong Linux

Tên biến cần được **VIẾT HOA** toàn bộ. Tên biến chỉ cho phép các ký tự ``a-z`` hoặc ``A-Z``, các số từ ``0-9`` và dấu gạch chân ``_``

Ví dụ về tên biến hợp lệ

```
_BIEN
BIEN_123
```

Tên biến không được bắt đầu bằng một chữ số và không được sử dụng các ký tự đặc biệt như ``!``,``*``,``-`` khi đặt tên biến

Ví dụ về tên biến không hợp lệ

```
1_BIEN
2AGE
BIRTH!
PHONE-NUMBER
```

### Định nghĩa và gán giá trị cho biến

Cấu trúc khai báo như sau:

``[tên_biến]=[giá_trị_biến]``

Ví dụ:

```
NAME="Vu The Vinh"
AGE=19
```

### Sử dụng

Để truy cập giá trị trong một biến bằng cách đặt ký tự ``$`` trước tên biến:

```
#!/bin/sh
NAME="Vu The Vinh"
AGE=19
echo $NAME $AGE
```

Kết quả:

``Vu The Vinh 19``

