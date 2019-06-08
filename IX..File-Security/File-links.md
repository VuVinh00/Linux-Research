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
