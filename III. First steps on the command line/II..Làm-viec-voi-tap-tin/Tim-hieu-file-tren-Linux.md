Trong Linux, tất cả mọi thứ ta tương tác đều là file. Mỗi file sẽ có 1 file descriptor để phân biệt (File descriptor là 1 số integer đại diện cho file). Hệ điều hành Linux phân biệt cách file bằng file descriptor.

Linux phân biệt chữ in hoa và chữ thường, hai file hay folder cùng tên nhưng khác kí tự in hoa hay in thường sẽ khác nhau

## Làm việc với tập tin

### Tạo tập tin mới - touch

Cú pháp : 
`touch <tên_file>`

### 2: Đổi tên, di chuyển file - mv

mv có 2 chức năng kép đó là di chuyển và đổi tên

#### 2.1: Đổi tên:

Cú pháp:
`mv <đường dẫn cũ với tên cũ> <đường dẫn mới với tên mới>`

Ví dụ đổi file test.txt thành new.txt
` mv /home/test.txt /home/new.txt `

#### 2.2: Di chuyển:
`mv <đường dẫn nguồn> <đường dẫn đích>`

Ví dụ muốn di chuyển tập tin test.txt ở /home sang /etc

`mv /home/test.txt /etc/test.txt`
