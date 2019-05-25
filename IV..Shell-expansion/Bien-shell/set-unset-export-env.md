### Hủy biến 

Để hủy một biến sử dụng lệnh ``unset`` với cú pháp:

``unset [tên_biến]``

Ví dụ hủy biến NAME:

```
#!/bin/sh
NAME="Vu The Vinh"
unset NAME
echo $NAME
```

Lệnh trên sẽ không in bất kì thông tin gì

### Xem danh sách biến trên hệ thống

Ta có thể xem danh sách hệ thống bằng lệnh **set** hoặc **env**

### Export 

--------

