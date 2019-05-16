## Sự khác biệt giữa dấu ngoặc đơn (' ') và dấu ngoặc kép (" ") trong Linux

Trước hết ta xem qua ví dụ này:

Đầu tiên ta đặt 1 biến ví dụ: ``ponet=luamoc``

Tiếp theo ta dùng lệnh **echo**:

-``$ echo "$ponet"`` nó sẽ in giá trị của biến **ponet** tức là **luamoc**

-``$ echo '$ponet'`` nó sẽ in ra ``$ponet`` ( chuỗi chính xác được truyền trong dấu nháy đơn )

--> Kết luận: dấu ngoặc kép (" ") được sử dụng để in giá trị bất kì của biến và dấu nháy đơn (' ') được sử dụng để in chuỗi chính xác.
