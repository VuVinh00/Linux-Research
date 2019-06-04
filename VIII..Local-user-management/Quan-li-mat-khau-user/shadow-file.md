### Shadow file : /etc/shadow

Mật khẩu user được mã hóa và lưu trữ tại **/etc/shadow**. File **/etc/shadow** là file chỉ đọc và chỉ có thể đọc bởi người dùng **root**. 

Cấu trúc file /etc/shadow:

``Username : Password-encode : last_pass_change : maxday : maximum : warn : inactive : expire ``

Ví dụ:

``root:$6$Dkwmavc$Aavdhvkwlhfwscdhfj/fwef:18051:0:999999:7::: ``

Giải thích:

**root** ( Username ): Tên người dùng

**$6$Dkwmavc$Aavdhvkwlhfwscdhfj/fwef** ( Password-encode ) : Mật khẩu được mã hóa, được phân cách thành 3 trường bởi **$**

``$6  $Dkwmavc   $Aavdhvkwlhfwscdhfj/fwef``

   - Trường 1 ( $1 ): Cho biết thuật toán mã hóa

        $1 : MD5
        
        $2 : blowfish

        $2a: eksblowfish

        $5 : sha256
        
        $6 : sha512
   - Trường 2 ( $Dkwmavc ): Là một chuỗi dữ liệu ngẫu nhiên (salt) kết hợp với pass người dùng, tăng tính bảo mật trong hàm băm
   - Trường 3 ( $Aavdhvkwlhfwscdhfj/fwef ) : Giá trị băm của salt + password
   
Nếu tại **password-encode** mà:

   - rỗng --> không có mật khẩu
   - !    --> mật khẩu người dùng bị chặn nhưng có thể sử dụng phương thức khác để connect như ssh key
   - *    --> mật khẩu bị chặn, vẫn có thể connect bằng phương thức khác 
