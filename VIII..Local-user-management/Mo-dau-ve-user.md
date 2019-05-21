## Các khái niệm cơ bản về quản lí user của Linux

Trong Linux có 2 phần đó là username và userID:

- **username**: Khi sử dụng để login, gán quyền, ... chúng ta thực hiện qua username nhưng hệ thống lại hiểu và làm theo userID

- **userID**: Là 1 số đi kèm username, hệ điều hành dùng số này để quản lý. Như vậy nếu có hai username khác nhau nhưng cùng chung một userID thì hệ thống sẽ xem hai tên này là một

## Các loại user:

Trong Linux chỉ phân biệt user làm hai loại:

- Supper user ( **root** ): Supper user có userID=0, đây là user có quyền cao nhất trong hệ thống, nó có thể làm được bất cứ thứ gì trên hệ thống của nó.
- Normal user : Tất cả những user có userID khác 0 đều là normal user
