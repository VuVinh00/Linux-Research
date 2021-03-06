### Quyền hạn là gì?

Quyền hạn là một phần quan trọng của linux có vai trò quan trọng trong việc nâng cao tính bảo mật và ổn định trên hệ thống linux. Mọi file trong Linux đều có các thuộc tính sau để thể hiện quyền hạn truy cập tới nó:
- Quyền hạn truy cập của người sở hữu : Quyền hạn truy cập của chủ nhân quyết định những hành động gì mà người sở hữu có thể thực hiện file
- Quyền hạn truy cập nhóm : Quyền hạn truy cập của nhóm quyết định hành động gì mà người sử dụng, thành viên của nhóm sở hữu file, có thể thực hiện trên file
- Quyền hạn truy cập khác: Chỉ hành động nào mà tất cả những người sử dụng có thể thực hiện trên file

### Quyền sở hữu file ( user owner and group owner)

**User** và **Group** của hệ thống được quản lí tại **/etc/passwd** và **/etc/group**. Các **user** và **group** có thể sở hữu các file và mọi file đều phải có người sở hữu và nhóm sở hữu

<img src="https://github.com/vjnkvt/Images/blob/master/owner.PNG">

Người dùng **paul** sở hữu 2 file, **file1** có người sở hữu là **paul** và nhóm sở hữu là **paul**, **data.odt** được sở hữu bởi nhóm **snooker**, file2 được sử hữu bởi nhóm **tennis**. File cuối cùng **stuff.txt** được sở hữu bởi người dùng **root** và nhóm **root**

### Quyền truy cập file 

Quền hạn truy cập file là dòng đầu tiên của sự bảo vệ trong hệ thống Linux. Các khối xây dựng cơ bản trong quyền hạn truy cập Linux là các quyền hạn truy cập đọc, ghi và thực thi

- Read : cho phép người dùng xem được nội dung trong file
- Write : cho phép người dùng xem, chỉnh sửa nội dung trong file
- Execute : cho phép chạy file, program.

#### Phân quyền 

Để xác định quyền hạn của 1 user, group người ta gắn một con số cho từng quyền: read ( r ) = 4, write ( w ) = 2, execute ( x) = 1 

| Quyền | Số | Ký hiệu |
|-------|----|------|
|Không đặt quyền | 0 | --- |
|Execute | 1 | --x |
|Write | 2 | -w- |
|Execute + Write| 3 | -wx |
|Read | 4 | r-- |
|Read + Execute |5| r-x |
|Read + Write |6| r-x |
|Read + Write + Execute | 7 | rwx |

Ví dụ: 
```
drwxr-xr-x.  4  root  root  64  May 13  08:25 Test
```

- d : đại diện cho folder
- r : read permission
- w : write permission
- x : execute permission

Quyền sẽ được hiển thị từ trái sang phải theo thứ tự : theo nhóm bị ảnh hưởng bởi quyền gồm : user - group - other

- Ở phần thứ nhất : user đang có full quyền rwx
- Ở phần thứ hai: group đang có quyền r-x là đọc và thực thi
- Ở phần thứ ba: other có quyền r-x là đọc và thực thi

### chgrp

- Là lệnh thay đổi nhóm sở hữu thư mục/ tập tin

``# chgrp [options] [group_owner] [file]``
    
  - Options:
    ``-R``: Áp dụng đối với thư mục làm cho lệnh ``chgrp`` có tác dụng trên các thư mục con
    
  - Group_owner: nhóm sở hữu mới của tập tin

### umask

Khi tạo file hoặc thư mục mới, quyền mặc định sẽ được áp dụng. Permissions mặc định được xác định bởi **umask**. **umask** xác định quyền 

### chmod

Là lệnh thay đổi quyền truy xuất trên thư mục / tập tin:

``# chmod [options] [mode] [file]``

  - **Options** :
  
    ``-R``: Áp dụng với mọi thư mục làm cho lệnh ``chmod`` có hiệu lực trên cả các thư mục con
  
  - **Mode** : Quyền truy xuất mới cho tập tin

### chown

Là lệnh thay đổi chủ sở hữu thư mục / tập tin ( owner )

``# chown [options] [owner] [file]``

   - **Options** : 
   
        ``-R``: Áp dụng đối với thư mục làm cho lệnh ``chown`` có tác dụng trên cả các thư mục con
   
   - **Owner**: chủ sở hữu mới của tập tin
   
