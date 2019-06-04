### Cách cấu hình Banner đăng nhập trong Linux ( CentOS 7 )

Ta có 2 cách cấu hình :
  
  **/etc/issue** : Sẽ xuất hiện trước khi người dùng đăng nhập
  
  **/etc/motd** : Sẽ xuất hiện sau khi người dùng đăng nhập

#### 1 : Để hiển thị banner trước khi user đăng nhập

Ta mở file **/etc/issue** sau đó sửa thành nội dung chúng ta muốn 

<img src="https://github.com/vjnkvt/Images/blob/master/issue.PNG">

#### 2 : Để hiện thị banner sau khi user đăng nhập

Ta mở file **/etc/motd** và sửa thành nội dung muốn sửa :

<img src="https://github.com/vjnkvt/Images/blob/master/motd.PNG">


### Sau khi khởi động lại hệ thống ta được banner như sau: 

<img src="">
