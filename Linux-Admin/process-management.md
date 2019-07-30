## Introduction to processes

### Process

Tiến trình ( process ) là quá trình biên dịch ( compile ) source code đang chạy trên hệ thống.

### PID 

Tất cả các tiến trình ( process ) đều có **process id ( PID )

### PPID 

Tất cả các tiến trình đều có tiến trình cha ( được gọi là **PPID**) . Tiến trình con thường được khởi động bằng tiến trình cha 

### init

Tiến trình **init** luôn có process ID ( **PID** ) là 1. Init process được khởi động bởi chính **kernel** vì vậy nó không có tiến trình cha ( parent process ).

### kill

Khi một tiến trình dừng chạy , tiến trình chết, khi muốn tiến trình chết thì ta sẽ **kill** chúng

### daemon

Các tiến trình được khởi động bởi hệ thống và chạy mãi mãi được gọi là tiến trình **daemon** . **daemon** không bao giờ chết

### zombie

Khi một tiến trình bị **kill** nhưng nó vẫn xuất hiện trên hệ thống, tiến trình đó được gọi là **zombie**. Không thể **kill** zombie bởi vì chúng đã chết.

### Basic process management

- $$
