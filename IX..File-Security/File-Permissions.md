### Quyền hạn là gì?

Quyền hạn là một phần quan trọng của linux có vai trò quan trọng trong việc nâng cao tính bảo mật và ổn định trên hệ thống linux. Mọi file trong Linux đều có các thuộc tính sau để thể hiện quyền hạn truy cập tới nó:
- Quyền hạn truy cập của người sở hữu : Quyền hạn truy cập của chủ nhân quyết định những hành động gì mà người sở hữu có thể thực hiện file
- Quyền hạn truy cập nhóm : Quyền hạn truy cập của nhóm quyết định hành động gì mà người sử dụng, thành viên của nhóm sở hữu file, có thể thực hiện trên file
- Quyền hạn truy cập khác: Chỉ hành động nào mà tất cả những người sử dụng có thể thực hiện trên file

### Quyền sở hữu file ( user owner and group owner)

**User** và **Group** của hệ thống được quản lí tại **/etc/passwd** và **/etc/group**. Các **user** và **group** có thể sở hữu các file và mọi file đều phải có người sở hữu và nhóm sở hữu

<img src="">
