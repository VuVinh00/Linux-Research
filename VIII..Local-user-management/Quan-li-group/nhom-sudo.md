### Giới thiệu về sudo

**Sudo** (Superuser Do) cho phép một user thực thi một lệnh bằng quyền root. Lý do chúng ta phải sử dụng **sudo** đó là:

  - Tăng cường tính bảo mật cho hệ thống
  - Quản lí quyền hạn của từng user hoặc group trong việc thực thi lệnh
  - Kiểm soát được user nào đã làm gì trên hệ thống 

Ví dụ một user bình thường sẽ không thể nào sử dụng các lệnh để dừng một tác vụ trên hệ thống. Nhưng nếu hộ gõ một lệnh dừng tác vụ nào đó mà có kèm chữ **sudo** đằng trước thì yêu cầu này sẽ được gửi đến hệ thống, hệ thống sẽ kiểm tra xem user đang gửi yêu cầu có nằm trong danh sách **sudoers** hay không, nếu có thì có phép thành viên kia thực thi còn không thì sẽ báo lỗi và lưu lại log

Đối với user gõ lệnh **sudo** thì sẽ được hỏi mật khẩu của chính họ để xác nhận.

### So sánh sudo và root

- **Root user** :
  
  Cả **su** và **sudo** đều được chạy với quyền của người dùng **root**. Người dùng **root** có quyền hạn tối đa và làm bất cứ thứ gì trong hệ thống. **Normal user** trên Linux thường có quyền hạn kém - ví dụ như normal user không thể cài đặt hay viết lên các thư mục hệ thống
  
  Để làm được điều gì khi bị yêu cầu quyền này thì ta phải sử dụng đến **sudo**
  
- **Sudo**:

**Sudo** chạy một lệnh duy nhất với quyền **root**. Khi ta thực thi câu lệnh **sudo**, hệ thống sẽ yêu cầu mật khẩu của người dùng hiện tại và chạy với tư cách người dùng root.
