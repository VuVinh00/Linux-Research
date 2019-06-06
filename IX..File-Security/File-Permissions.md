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

