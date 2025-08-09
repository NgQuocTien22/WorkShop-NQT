---
title : "Tạo Directory Service"
date: "2025-07-11"
weight : 3 
chapter : false
pre : " <b> 3. </b> "
---


#### Tạo **Directory Service**

Ở thanh tìm kiếm của **AWS Console** search **Directory Service**

![DirectoryService](/images/3.directoryservice/001-ds.png)

Ở thanh task bên trái chọn **Directories** và bấm chọn **Set up Directory**

![DirectoryService](/images/3.directoryservice/002-ds.png)

+ Chọn Simple AD ( phù hợp với dự án nhỏ và nội bộ) sau đó bấm **Next**

![DirectoryService](/images/3.directoryservice/003-rt.png)

Sau đó ở trang enter **Directory Information** nhập các thông tin cần thiết

Phần Diretory size nên chọn **Small** vì sẽ phù  hợp với dự án nhỏ

![DirectoryService](/images/3.directoryservice/004-ds.png)

Sau khi đến trang Choose VPC and subnet 
+ Chọn VPC và Subnet đã tạo
+ Sau đó bấm **Next**

![DirectoryService](/images/3.directoryservice/005-ds.png)

Sau đó sẽ được chuyển tới trang review hãy kiểm tra lại các thông tin bạn đã điền sau đó bấm **Create Directory**

![DirectoryService](/images/3.directoryservice/006-ds.png)

Sau khi bấm tạo phải chờ từ 15-30 phút để AWS triển khai AD hãy check status đến khi có chữ Active sẽ tiến hành bước tiếp theo 
![DirectoryService](/images/3.directoryservice/007-ds.png)

Sau khi Status chuyển sang Active tiến hành Tạo người dùng “AdminUser” và gán quyền domain admin ( khi đăng nhập WorkSpaces sẽ có toàn quyền)
