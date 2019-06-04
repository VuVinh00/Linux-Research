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

### 4: groupmod

Ta có thể sửa tên group bằng câu lệnh **groupmod**

Cú pháp:

``$ groupmod -n [newgroup] [oldgroup]``

### 5: gpasswd

Ta có thể ủy quyền điều khiển group cho một người trong group bằng câu lệnh **gpasswd**.

**gpasswd** cũng dùng để xóa tất cả quản trị viên khỏi một nhóm, hãy sử dụng lệnh **gpasswd** để đặt trống danh sách quản trị viên 

``$ gpasswd -A "" [tên-group]``

### 6: newgrp

### 7: vigr

**vigr** được dùng để sửa thủ công file **/etc/group**. Chỉ những quản trị viên cấp cao đã có kinh nghiệm mới nên sử dụng **vi** hoặc **vigr** để quản lí group.
