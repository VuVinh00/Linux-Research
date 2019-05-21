### Câu lệnh whoami

**whoami** sẽ cho ta biết ta đang làm việc với user nào

Cú pháp:

``$ whoami``

Ví dụ:

```
$ whoami
root
```

### Câu lệnh who

**who** giúp liệt kê những người dùng đang đăng nhập hiện tại trên hệ thống.

Cú pháp:

``$ who``

### Câu lệnh w

**w** liệt kê những user đã đăng nhập và họ đang làm gì

Ví dụ:

``$ w``

Output:

<img src="https://github.com/vinhvt2704/Images/blob/master/w.PNG">

### Câu lệnh id 

**id** show ra uid, gid và groups của user

Cú pháp:

``$ id [user]``

Ví dụ:

``$ id root``

Output:

<img src="https://github.com/vinhvt2704/Images/blob/master/id.PNG">

## Câu lệnh su

Nói tóm gọn thì **su** giúp chúng ta đăng nhập sang 1 user khác ngay trên terminal đang chạy.

Cú pháp:
``$ su [username]``

Ví dụ:

<img src="https://github.com/vinhvt2704/Images/blob/master/su.PNG">

## Câu lệnh sudo

Lệnh **sudo** cho phép một user có thể thực hiện chạy lệnh nào đó trong hệ thống dưới dạng người dùng cao nhất hoặc người dùng khác

Ví dụ khi ta đang ở user thường sẽ không thể chạy lệnh **shutdown** nhưng khi ta thêm sudo ở trước ``sudo shutdown`` thì câu lệnh sẽ lập tức được thực hiện

## Câu lệnh visudo

**visudo** dùng để sửa file sudoers, file này định nghĩa các câu lệnh và các user có thể chạy với quyền sudo

