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

Ngược lại với **head**, câu lệnh **tail** cho phép chúng ta xem phần cuối nội dung của file. Câu lệnh **tail** rất hữu dụng trong trường hợp chúng ta muốn xem nội dung của các file log của chương trình vì thông thường với các file log này chúng ta chỉ muốn xem thông báo lỗi gần đây thay vì xem toàn bộ các lỗi.

Cú pháp:

``$ tail <tên-file>``

Ví dụ: 

``$ tail sample.txt``

Mặc định câu lệnh **tail** sẽ hiển thị 10 dòng cuối có trong file. Nếu muốn chỉnh số lượng dòng hiển thị thì có thể sử dụng tùy chọn **-n** trong câu lệnh như sau:

``tail -n <tên-file>``

Ví dụ: 

``tail -20 sample.txt``

Ngoài ra, ta có thể sử dụng tùy chọn **-f** trong câu lệnh **tail** để xem nội dung của file log theo kiểu thời gian thực (real time).

``$ tail -f /var/log/apache2/access.log``

### cat

Khác với **head** hay **tail**, câu lệnh **cat** sẽ hiển thị toàn bộ nội dung của file.

Cú pháp:

``$ cat <tên-file>``

Ví dụ:

``$ cat sample.txt``

### more 

Câu lệnh **more** được sử dụng để mở nội dung của file. Nếu nội dung của file quá lớn nó sẽ hiển thị theo từng trang. Ta có thể dùng nút **Enter** hoặc **Space** để cuộn trang. Nhưng câu lệnh **more** chỉ có thể cuộn xuống, không thể cuộn lên.

Cú pháp:

``$ more <tên-file>``

Ví dụ:

``more sample.txt``

Để tìm kiếm một chuỗi, ta gõ phím ``/`` rồi nhập từ cần tìm kiếm và gõ **Enter**

``/Search``

### less

Câu lệnh **less** hiển thị nội dung của toàn bộ file. Không giống như **more**, câu lệnh **less** có thể cuộn lên và cuộn xuống.

Cú pháp:

``$ less <tên-file>``

Ví dụ:

``$ less sample.txt``

Để tìm kiếm một chuỗi, cũng như **more** ta gõ phím ``/`` rồi nhập từ cần tìm kiếm và gõ **Enter**

``/Search``
