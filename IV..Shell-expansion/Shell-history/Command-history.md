## Cách sử dụng lệnh history

Khi ta gõ ra màn hình lệnh **history**, hệ thống sẽ in ra màn hình lịch sử những câu lệnh mà user hiện tại đã thực hiện trước đó.

### Thực thi lại câu lệnh gần nhất

Để thực hiện lại câu lệnh gần nhất, ta gõ 2 dấu **!!**

Ví dụ:

<img src="https://github.com/vjnkvt/Images/blob/master/!!.PNG">

### Thực hiện lại câu lệnh thứ n

Để thực hiện lại câu lệnh thứ **n** trong lịch sử câu lệnh các bạn sử dụng cú pháp **!n**

Ví dụ:

<img src="https://github.com/vjnkvt/Images/blob/master/!n.PNG">

### Tổ hợp phím "Ctrl + R"

Một lựa chọn khác để tìm kiếm lịch sử là sử dụng **Ctrl + R**. Nhấn **Ctrl + R** sau đó bắt đầu gõ một phần của câu lệnh, hệ thống sẽ tự hoàn tất phần còn lại dựa trên các câu lệnh đã được thực hiện trước đó.

### $HISTSIZE

Biến **HISTSIZE** xác định số lượng lệnh được lưu trong môi trường hiện tại. Hầu hết các bản phân phối hiện nay mặc định từ 500 đến 1000

<img src="https://github.com/vjnkvt/Images/blob/master/histzise.PNG">

Ta có thể thay đổi giá trị này như sau:

<img src="https://github.com/vjnkvt/Images/blob/master/9999.PNG">

### $HISTFILE

Biến **HISTFILE** là nơi lưu trữ lịch sử câu lệnh. Mặc định được lưu ở **~/.bash_history**

Lịch sử phiên được lưu vào file này khi bạn thoát khỏi phiên

*Đóng màn hình dòng lệnh gnome bằng chuột hoặc **reboot** sẽ không lưu lại lịch sử câu lệnh*

### $HISTFILESIZE

Số lượng command sẽ được giữ lại trong file, ta cũng có thể thay đổi giá trí này như **$HISTSIZE**
