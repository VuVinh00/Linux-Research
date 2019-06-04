### System profile

Cả hai **bash** và **ksh** shell sẽ xác minh sự tồn tại của **/etc/profile** và mã nguồn của nó nếu tồn tại

Khi đang đọc script, bạn sẽ nhận thấy nó xây dựng trên biến môi trường **PATH**. Script cũng có thể thay đổi biến **PS1**, đặt tên **HOSTNAME** và thực thi một số scripts như **/etc/inputrc**

Sử dụng grep để hiển thị thao tác trong **/etc/profile** trên Centos7

<img src="https://github.com/vjnkvt/Images/blob/master/systemprofile.PNG">

Người dùng **root** có thể sử dụng script để set **aliases**, **functions** and **variables** cho mọi user trên hệ thống.

### ~/.bash_profile

Khi file này tồn tại ở thư mục home, thì **bash** sẽ có nguồn của nó. Ở bản Debian Linux 5/6/7 thì mặc định file này không tồn tại

CentOS 7 sử dụng **~/.bash_profile**, nơi nó sẽ kiểm tra sự tồn tại của **~/.bashrc**. Nó cũng thêm **$HOME/bin** vào biến **$PATH**

<img src="https://github.com/vjnkvt/Images/blob/master/bash_profile.PNG">

### ~/.bash_login

Chứa các cài đặt cụ thể được thực thi khi người dùng đăng nhập vào hệ thống. **.bash_login** sẽ được thực thi khi **.bash_profile** không tồn tại

### ~/.profile

Khi cả **~/.bash_profile** và **~/.bash_login** đều không tồn tại, **bash** sẽ xác minh sự tồn tại của **~/profile** và thực thi nó. File này mặc định không tồn tại trên RHEL, CentOS

### ~/.bashrc

**~/.bashrc** là một shell script file, thường được sử dụng như một tệp cấu hình riêng cho 1 người dùng cụ thể

Vị trí của nó ở home directory và được thực thi khi user đăng nhập vào bash

Nó thường được sử dụng để set tùy chỉnh của người dùng ( user preferences) hoặc biến mỗi trường ( environment variables) nhưng không chỉ giới hạn ở đó, vì nó là file shell script nên nó cũng có thể được sử dụng để chạy bất cứ thứ gì user có thể chạy

### ~/.bash_logout

Khi thoát phiên làm việc bash, nó có thể thực thi **~/.bash_logout

