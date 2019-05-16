# Các loại Command line trên LINUX

## Tìm ra loại lệnh ( type -t )

Nếu ta dùng type -t thì nó sẽ in ra một từ thuộc trong những từ dưới đây:
 - alias ( nghĩa là shell alias )
 - keyword ( nghĩa là shell reserved word )
 - function ( nghĩa là shell function )
 - builtin ( nghĩa là shell builtin )
 - file ( nghĩa là disk file )

Ví dụ:

Command | Output | Ý nghĩa
--- | --- | ---
type -t ls | alias | Là tên rút gọn của command, thay vì phải nhập lệnh đầy đủ của ls thì chúng ta chỉ cần nhập là ls
type -t pwd | builtin | Là lệnh được xây dựng bên trong vỏ của nó, những lệnh này có thể dùng khi hệ thống bị crash hoặc không thể truy cập được vào máy tính
type -t date | file | Là các lệnh bên ngoài được lưu trữ tại: /bin /usr/bin /usr/local/bin /sbin /usr/sbin /usr/local/sbin
type -t xrpm | function | Là một hàm do người dùng tự định nghĩa
type -t if | keyword | Là câu lệnh đặc biệt dùng trong shell |

## Tìm đường dẫn của câu lệnh ( type -p )

Type -p dùng để tìm ra đường dẫn của disk file. Nó sẽ không trả lại gì nếu câu lệnh đó không phải loại disk file

Ví dụ:

Ta dùng lệnh:

`` type -p ls ``

Sẽ không trả ra kết quả gì bởi ls thuộc type alias. Chúng ta có thể kiểm tra lại bằng lệnh **type -t ls**

Giờ thử dùng **type -p** với câu lệnh thuộc loại disk file là **date**

`` type -p date``

Ta sẽ có kết quả tương tự:

``bin/date``

## Tìm kiếm tất cả thông tin về câu lệnh ( type- a )

Type -a có thể được sử dụng để tìm kiếm câu lệnh là disk file, alias, keyword or function. Nó sẽ cho ta tất cả thông tin về câu lệnh như loại của câu lệnh, đường dẫn của câu lệnh,...

Ví dụ:

`` type -a pwd ``

Kết quả sẽ là :

``` 
pwd is a shell builtin
pwd is /bin/pwd
```
