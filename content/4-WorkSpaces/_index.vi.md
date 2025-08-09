---
title : "Tạo WorkSpaces"
date: "2025-07-11"
weight : 4 
chapter : false
pre : " <b> 4. </b> "
---


#### Tạo **WorkSpaces**
1. Trong **AWS Console** search **WorkSpaces** trên thanh tìm kiếm 

![WorkSpaces](/images/4.workspaces/001-ws.png)

Ở thanh task bên trái 
+ Bấm vào Directories
+ Sau đó bấm Create Directory
![WorkSpaces](/images/4.workspaces/002-ws.png)

Chọn cấu hình như ảnh dưới đây 

![WorkSpaces](/images/4.workspaces/003-ws.png)

+ Sau đó bấm Register 
+ Sau khi đăng ký thành công đợi 1 lúc để AWS xử lý 

2. Trong giao diện **WorkSpaces** chọn **Personal**
+ Sau đó chọn **Create WorkSpaces**

![WorkSpaces](/images/4.workspaces/004-ws.png)

Ở giao diện **Onboading - optional** Cấu hình như ảnh sau

![WorkSpaces](/images/4.workspaces/005-ws.png)

Sau khi xong bấm **Next**

Bạn sẽ được đưa tới bước **Configure WorkSpaces**
+ Cấu hình như trong ảnh 
![WorkSpaces](/images/4.workspaces/006-ws.png)

Sau đó bấm **Next**

Sẽ tới bước tiếp theo là **Select Directory**

+ Tiếp theo chúng ta sẽ cấu hình máy ảo 
+ Chọn Bundle (Gói cấu hình phần cứng + OS)
+ Chọn bundle có tên:
    Performance with Windows 10 (Server 2022 based)
+ Ví dụ cấu hình đi kèm: 2 vCPU, 8 GB RAM, Protocol: WSP, Có cài sẵn Mozilla Firefox, Ngôn ngữ: English.

(Note: Nếu chưa có user thì bấm create user để tạo 1 user)

Sau đó bấm **Next**

![WorkSpaces](/images/4.workspaces/007-ws.png)

Ở bước cuối Customization kiểm tra lại các option đã chọn ( có thể sửa tùy theo nhu cầu)
Sau đó bấm **Create WorkSpaces**
![WorkSpaces](/images/4.workspaces/008-ws.png)

Chờ 1 lúc AWS sẽ gửi cho bạn 1 mail có chứa thông tin đăng nhập và link đổi mật khẩu 

![WorkSpaces](/images/4.workspaces/009-ws.png)

Sau khi đổi mật khẩu xong tiến hành đăng nhập vào WorkSpaces
+ Nhập Code được gửi trong gmail
+ Sau đó bấm **Continue**
![WorkSpaces](/images/4.workspaces/010-ws.png)

Sau đó bạn sẽ đăng nhập bằng tài khoản đã tạo 
![WorkSpaces](/images/4.workspaces/011-ws.png)

Sau khi đăng nhập thành công bạn sẽ được đưa vào máy ảo 
![WorkSpaces](/images/4.workspaces/012-ws.png)

Tiến hành kiểm tra xem đã có quyền Admin chưa 
+	Mở Start menu
+	Gõ và mở: Computer Management
+	Vào Local Users and Groups → Groups
+	Click vào Administrators
Nếu thấy user TIENLAB\adminuser có trong thì đã có đầy đủ quyền admin 
![WorkSpaces](/images/4.workspaces/013-ws.png)

Sau đó tiến hành chạy thử trên môi trường máy ảo bằng cách kiểm tra kết nối internet và cài đặt thử các công cụ hỗ trợ học tập (Ở đây mình đã tải thử Visual Code)

![WorkSpaces](/images/4.workspaces/014-ws.png)

Đánh giá : Có thể thấy mạng và tốc độ khá ổn định có thể hỗ trợ công việc rất tốt.