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

        $1 : MD5\n
        $2 : blowfish

        $2a: eksblowfish

        $5 : sha256
        
        $6 : sha512
