## Các câu lệnh xem nội dung File

### head

Câu lệnh head trong linux cho phép chúng ta xem phần đầu nội dung của file

Cú pháp:

``$ head <tên-file>``

Ví dụ:

``$ head sample.txt``

Mặc định thì câu lệnh **head** sẽ hiển thị 10 dòng đầu tiên có trong file. Nếu muốn chỉnh số lượng dòng hiển thị thì có thể sử dụng tùy chọn **-n** trong câu lệnh như sau:

``$ head -n <tên-file>``

Ví dụ:

`` head -20 sample.txt ``

### tail

Ngược lại với **head**, câu lệnh **tail** cho phép chúng ta xem phần cuối nội dung của file.

Cú pháp:

``$ tail <tên-file>``

Ví dụ: 

``$ tail sample.txt``

Mặc định câu lệnh **tail** sẽ hiển thị 10 dòng cuối có trong file. Nếu muốn chỉnh số lượng dòng hiển thị thì có thể sử dụng tùy chọn **-n** trong câu lệnh như sau:

``tail -n <tên-file>``

Ví dụ: 

``tail -20 sample.txt``
