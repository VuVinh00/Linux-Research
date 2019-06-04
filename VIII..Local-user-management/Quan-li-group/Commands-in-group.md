### 1: groupadd

Group có thể được tạo với câu lệnh **groupadd**.

Cú pháp :

``$ groupadd [tên+group]``

### 2: groupdel

Ta có thể xóa một group vĩnh viễn bằng câu lệnh **groupdel**

Cú pháp:

``$ groupdel [tên+group]``

### 3: usermod

Thành viên nhóm có thể được sửa đổi bằng câu lệnh **usermod**

Cẩn thận khi sử dụng **usermod** để add user vào groups. Bởi mặc định thì **usermod** sẽ xóa tất cả user từ mọi group mà user đó làm thành viên nếu như không được liệt kê trong câu lệnh. Sử dụng option **-a** để ngăn chặn hành động này

### 4: Groupmod

Ta có thể sửa tên group bằng câu lệnh **groupmod**

Cú pháp:

``$ groupmod -n [newgroup] [oldgroup]``

### gpasswd
