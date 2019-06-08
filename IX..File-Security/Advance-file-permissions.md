### Sticky

- Được dùng cho các thư mục chia sẻ, mục đích là ngăn chặn việc người dùng này xóa file của người dùng kia. Chỉ duy nhất **owner file** và **root** mới có quyền rename hay xóa các file, thư mục khi nó được set **sticky bit**

- **Sticky bit** được mô tả bằng chữ cái ``T`` ở cuối dòng hiển thị permission:

``-rw-r---r-T.  1 root  root    0 Jun 9:00  test.txt``

- Cách thêm **Sticky bit**:

``# chmod o+t [file]``

hoặc

``# chmod 1750 [file]``
