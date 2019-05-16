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

### tailf

**tailf** là một câu lệnh đã không được dùng nữa. Nó đã được thay bằng câu lệnh **tail -f**.

**tailf** sẽ in ra 10 dòng cuối trong file và sau đó sẽ đợi file lớn lên. Nó giống với **tail -f** nhưng nó sẽ không truy cập vào file khi file đó không lớn lên.

Cú pháp:

``$ tailf <tên-file>``

Ví dụ:

``$ tailf sample.txt``

### cat

Khác với **head** hay **tail**, câu lệnh **cat** sẽ hiển thị toàn bộ nội dung của file.

Cú pháp:

``$ cat <tên-file>``

Ví dụ:

``$ cat sample.txt``

### tac

**tac** ngược lại câu lệnh với **cat**, nếu như **cat** in ra toàn bộ file từ trên xuống thì **tac** cũng in ra toàn bộ file nhưng sẽ hiển thị từ dưới lên trên

Cú pháp:

``$ tac <tên-file>

Ví dụ:

``$ tac example.txt

Đây là hình ảnh so sánh giữa cat và tac

<img src="https://github.com/vinhvt2704/Images/blob/master/tac-basic-usage.png">

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

## strings

Câu lệnh **strings** dùng để đọc các ký tự nhị phân trong văn bản. Đã bao giờ bạn cố gắng chạy một tệp nhị phân ( binary file ) bằng lệnh như là **cat** và thấy kết quả không mong muốn. Nếu chưa thử chạy tệp nhị phân bằng lệnh **cat** thì bạn có thể thử bằng cách sau đây:

Đầu tiên ta tìm đường dẫn của 1 tệp nhị phân, ví dụ như:
``$ which cat``

Output:

``/bin/cat`` ( Lưu ý: kết quả này có thể khác đối với bản Linux của bạn)

Sau đó chúng ta thử dùng lệnh **cat** để đọc tệp nhị phân này:

``$ cat /bin/cat``

Như bạn có thể thấy, nó sẽ hiện ra toàn kí tự kì lạ và nó không như mong đợi khi bạn muốn đọc 1 file đó. Bây giờ ta hãy thử dùng câu lệnh **strings** để đọc tệp nhị phân ``/bin/cat`` bằng câu lệnh:

``strings /bin/cat``

Bây giờ chúng ta có thể nhìn thấy sự khác biệt khi ta đọc tệp nhị phân bằng câu lệnh **cat** và **strings**.

### echo

Câu lệnh **echo** được sử dụng để hiển thị dòng văn bản ra màn hình. Câu lệnh **echo** thường được sử dụng trong shell scripts và file batch để in ra trạng thái ra màn hình hoặc 1 tệp

Ví dụ để in một chuỗi văn bản, chúng ta có thể dùng lênh echo như sau:

```
$ echo "Sampleeeee"
Sampleeeee"
```
