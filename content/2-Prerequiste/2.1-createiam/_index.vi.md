---
title : "Tạo IAM Role"
date: "2025-07-11"
weight : 1 
chapter : false
pre : " <b> 2.1 </b> "
---

#### Tạo **IAM User để đảm bảo người vận hành có thể tạo, cấu hình, giám sát WorkSpaces**
1. Truy cập vào AWS Console tìm kiếm IAM 
![iam](/images/2.prerequisite/001-Role.png)

Ở thanh task bên trái chọn User
![iam](/images/2.prerequisite/002-Role.png)

Sau đó bấm chọn Create User
![iam](/images/2.prerequisite/003-Role.png)
 
Tiến hành đặt tên và tích chọn vào Provide user access to the AWS Management Console
Bạn có thể chọn tự tạo mật khẩu hoặc để AWS tự tạo cho bạn sau đó bấm **Next** 
Bạn sẽ được đưa tới giao diện setpermissions
Chọn các lựa chọn như trong ảnh 
Chọn 5 permissions như sau 
+ **AdministratorAccess** 
+ **AmazonWorkSpacesAdmin**
+ **IAMReadOnlyAccess**
+ **CloudWatchReadOnlyAccess**
+ **AmazonSSMFullAccess**

sau đó bấm **Next**

![createpolicy](/images/2.prerequisite/001-IAMROLE.png)
Xem và kiểm tra kỹ các lựa chọn
![createpolicy](/images/2.prerequisite/004-role.png)

Sau khi thành công mà hình sẽ hiển thị như sau 
![iam](/images/2.prerequisite/005-role.png)
có thể chọn tải Download .csv file để lưu lại tài khoản 

Sau đó copy link ở phần **Console sign-in URL** 
![iam](/images/2.prerequisite/005.1-role.png)

Sau đó tiến hành đăng nhập vào account được cung cấp và tiến hành đổi mật khẩu 
![iam](/images/2.prerequisite/004-IAMROLE.png)

Sau khi đăng nhập thành công tiến hành các bước tiếp theo 

