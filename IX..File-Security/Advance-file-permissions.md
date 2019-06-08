### Sticky

- Được dùng cho các thư mục chia sẻ, mục đích là ngăn chặn việc người dùng này xóa file của người dùng kia. Chỉ duy nhất **owner file** và **root** mới có quyền rename hay xóa các file, thư mục khi nó được set **sticky bit**

- **Sticky bit** được mô tả bằng chữ cái ``T`` ở cuối dòng hiển thị permission:

``-rw-r---r-T.  1 root  root    0 Jun 9:00  test.txt``

- Cách thêm **Sticky bit**:

``# chmod o+t [file]``

hoặc

``# chmod 1750 [file]``

- Xóa **Sticky bit**:

``chmod u-s [file]``

### SUID ( Set user ID )

- **SUID** được sử dụng trên các file thực thi (**executable files**) để cho phép việc thực thi được thực hiện dưới **owner file** thay vì thực hiện như user đang login trong hệ thống

- **SUID** cũng có thể được sử dụng để thay đổi ownership của file được tạo

- Cách thêm **SUID**:

``# chmod u+s [file]``

hoặc 

``# chmod 4750 [file]``

- Xóa **SUID**:

``chmod u-s [file]``

### SGID ( Set group ID )

- **SGID** cũng tương tự như **SUID** được sử dụng trên các file thực thi được thực hiện dưới **owner group** của file

- **SGID** cũng có thể được sử dụng để thay đổi **ownership group** của file được tạo

- Cách thêm **SGID**:

``# chmod g+s [file]``

hoặc

``# chmod 2750 [file]``

- Xóa **SGID**:

``# chmod g-s [file]``
