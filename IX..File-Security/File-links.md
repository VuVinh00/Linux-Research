## Inodes 

**Inodes** (**index node**) là 1 cấu trúc dữ liệu chứ các metadate của file, thư mục trong các hệ thống file trong Linux

Trong 1 **inode** gồm :
  - Dung lượng file ( byte )
  - **Device ID**: mã số thiết bị lưu file
  - **User ID**: mã số owner của file
  - **Group ID**: mã số group sở hữu file
  - **File mode**: gồm kiểu file và permission
  - Hệ thống phụ và các cờ hạn chế quyền truy cập file
  - **Timestamps**: các mốc thời gian khi: bản thân inode bị thay đổi (**ctime**), nội dung file bị thay đổi (**mtime**) và lần truy cập mới nhất (**atime**)
  - **Link count**): số lượng **hard link** trỏ đến **inode**
  - Các con trỏ ( từ 11 đến 15 con trỏ ) chỉ đến các block trên ổ cứng dùng để lưu trữ nội dung file. Theo các con trỏ này mới biết file nằm ở đâu để đọc nội dung
  
Các lệnh kiểm tra **inode**:

  - Show số **inode**:
    
    ``# ls -i [đường_dẫn_file]``
    
  - Cho biết chi tiết nội dung **inode**
  
    ``# stat [đường_dẫn_file]``

## About directories

### Directory

Thư mục ( directory ) là một loại tập tin đặc biệt chứa bảng ánh xạ các filename tới inodes

### . and ..

<img src="https://github.com/vjnkvt/Images/blob/master/direc.PNG">

Như hình trên ta có 5 filename và được ánh xạ tới 5 inodes. Dấu chấm **.** là ánh xạ cho chính nó ( thư mục hiện hành) và hai dấu chấm **..** được ánh xạ tới cha của thư mục hiện hành. 3 filename còn lại được ánh xạ tới các inodes khác

## Hard link và symbolic link

Trong 1 hệ thống file, mỗi file có 1 và chỉ 1 **inode**, mỗi **inode** cũng chỉ có 1 số inode duy nhất. Nhưng 1 file có thể có nhiều tên file tùy theo số **hard link** trỏ đến nó

### Hard link

- Là 1 liên kết ( link ) trỏ đến vị trí lưu 1 file trên ổ cứng
- Nếu đổi tên, xóa hoặc di chuyển file gốc sang thư mục khác, **hard link** vẫn được mở file đó vì nó vẫn trỏ đến vị trí lưu file cố định trên ổ cứng 
- Tên **hard link** có thể khác tên file gốc, **hard link** có thể nằm trong 1 thư mục khác với thư mục của file gốc. Vì vậy, 1 file có thể có nhiều tên file nằm ở các thư mục khác nhau. Khi truy cập vào **hard link** sẽ truy cập thằng đến file ( mở file hoặc thực thi file )
- Nếu đồng thời mở 1 file từ các **hard link** và tên file gốc, khi sửa ở 1 bản, các bản khác cũng thay đổi theo sau khi refresh hoặc reload vì thực chất là sửa trên cùng 1 file
- Nếu muốn xóa 1 **hard link** hoặc xóa tên file gốc nhưng còn 1 **hard link**, file vẫn không bị xóa. File chỉ bị xóa khi không còn gì trỏ đến vị trí lưu nó ( Muốn xóa 1 file, phải xóa tên file và tất cả các **hard link** của nó
- **Hard link** không tạo được với thư mục và không tạo được với file nằm trên partition khác 
- **Hard link** được tạo bởi lệnh ``ln``:

``# ln [path/file_name] [hardlink_name]``

### Symbolic Link

- Còn được gọi là **Soft Link** hoặc **symlink**
- Là 1 liên kết tạo ra 1 đường dẫn khác đến thư mục hoặc file gốc 
- Ví dụ file gốc **passwd** có đường dẫn là ``/etc/passwd``. Trong thư mục ``/home/user`` tạo ra 1 **soft link** đặt tên là ``password`` trỏ đến file đó thì khi truy cập 1 trong 2 đường dẫn đều là truy cập đến file ``passwd``
- Nếu đổi tên, xóa hoặc di chuyển file gốc sang thư mục khác thì **soft link** bị mất tác dụng, không truy cập được đến file đó nữa
- **Soft link** được tạo bởi lệnh ``ln -s``:

``# ln -s [path/file_name] [softlink_name]``
