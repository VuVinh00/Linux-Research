### System profile

Cả hai **bash** và **ksh** shell sẽ xác minh sự tồn tại của **/etc/profile** và mã nguồn của nó nếu tồn tại

Khi đang đọc script, bạn sẽ nhận thấy nó xây dựng trên biến môi trường **PATH**. Script cũng có thể thay đổi biến **PS1**, đặt tên **HOSTNAME** và thực thi một số scripts như **/etc/inputrc**

Sử dụng grep để hiển thị thao tác trong **/etc/profile** trên Centos7

<img src="https://github.com/vjnkvt/Images/blob/master/systemprofile.PNG">

Người dùng **root** có thể sử dụng script để set **aliases**, **functions** and **variables** cho mọi user trên hệ thống.

### ~/.bash_profile

Khi file này tồn tại ở thư mục home, thì **bash** sẽ có nguồn của nó. Ở bản Debian Linux 5/6/7 thì mặc định file này không tồn tại

CentOS 7 sử dụng **~/.bash_profile**, nơi nó sẽ kiểm tra sự tồn tại của **~/.bashrc**. Nó cũng thêm **$HOME/bin** vào biến **$PATH**

<img src="">

### ~/.bash_login

Chứa các cài đặt cụ thể được thực thi khi người dùng đăng nhập vào hệ thống. **.bash_login** sẽ được thực thi khi **.bash_profile** không tồn tại

### ~/.profile

Khi cả **~/.bash_profile** và **~/.bash_login** đều không tồn tại, **bash** sẽ xác minh sự tồn tại của **~/profile** và thực thi nó. File này mặc định không tồn tại trên RHEL, CentOS

### ~/.bashrc

