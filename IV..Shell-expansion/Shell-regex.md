### Regular Expression là gì?

**Regex** ( viết tắt của Regular Expression, tên thuần Việt là biểu thức chính quy) là một chuỗi các kí tự miêu tả một bộ các chuỗi kí tự khác, theo những quy tắc và cú pháp nhất định. **Regex** thường được sử dụng bởi các lệnh khác nhau như ed, sed, awk, grep, ...

**Regex** mang đến khả năng tìm kiếm xâu ký tự mạnh mẽ cho bất cứ công cụ xử lý text nào, trong Linux bạn sẽ không có được sự mạnh mẽ của các filter như GREP, EGREP hay các editor khác nếu bạn không làm chủ được **Regex**

### Basic regex:

| Ký hiệu | Mô tả |
|-----------|---|
|^      |Khớp đầu chuỗi |
|$      |Khớp cuối chuỗi |
|*      |Khớp với 0 hoặc nhiều lần ký tự trước|
|( )    |Nhóm biểu thức chính quy|
|?      |Khớp tối đa 1 ký tự|

Ví dụ: Ta có thư mục **Test** bao gồm các thư mục sau:

<img src="">

- Ký tự ^ : Tìm kí tự bắt đầu của một chuỗi 

<img src="https://github.com/vjnkvt/Images/blob/master/%5E.PNG">

- Ký tự $ : Tìm kí tự cuối của một chuỗi

<img src="">
