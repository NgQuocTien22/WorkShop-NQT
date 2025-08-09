---
title : "Tiến hành bảo mật và theo dõi hiệu suất"
date: "2025-07-11"
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

### **Tiến hành bảo mật và kiểm tra hiệu suất**

1. Trong giao diện của **AWS Console** search **EC2**.
![ec2](/images/5.sap/001-sap.png)

Ở thanh task bên trái tìm **Sercurity Group**
![ec2](/images/5.sap/002-sap.png)

Bấm **Create Sercurity Group**
![ec2](/images/5.sap/003-sap.png)
.
Tích chọn vào **Sercurity Groups** đã gán cho WorkSpaces -> sau đó chọn **Edit Inbound rules**

![ec2](/images/5.sap/004-sap.png)

Thêm các rules như sau:

![ec2](/images/5.sap/005-sap.png)

Sau đó bấm **Save Rules**

2.  Sau đó đến bước Enable CloudTrail để ghi log hoạt động.
Trong giao diện **AWS Console** search **CloudTrail**
![cloudtrail](/images/5.sap/006-sap.png)

Chọn **Create a trail**
![cloudtrail](/images/5.sap/007-sap.png)

Tiến hành tạo
![cloudtrail](/images/5.sap/008-sap.png)

3. Ở thanh tìm kiếm search **CloudWatch** ở thanh task bên trái chọn **Logs** -> **Logs Group**.

![cloudwatch](/images/5.sap/009-sap.png)

Tiến hành thêm thông tin vào các ô yêu cầu 
![cloudwatch](/images/5.sap/010-sap.png)

Sau đó bấm **Create**

4. Tiến hành gán nó vào **CloudTrail** để ghi lại các sự kiện đăng nhập, cấu hình và hoạt động người dùng trên **AWS WorkSpaces**.

Trước đó hãy tiến hành tạo role có chứa **CloudTrail** trước
Trong giao diện **AWS Console** truy cập vào **IAM**
![iam](/images/2.prerequisite/006-role.png)

Cấu hình như trong ảnh dưới đây 
![iam](/images/2.prerequisite/007-role.png)

Tìm và chọn policy giống ảnh 
![iam](/images/2.prerequisite/008-role.png)

Ở trang review hãy kiểm tra lại và bấm **Create Roles**
![iam](/images/2.prerequisite/009-role.png)

Sau đó quay lại CloudTrail -> Trail đã tạo 

![cloudtrail](/images/5.sap/011-sap.png)

Ở phần CloudWatch Logs chọn Edit  
Thiết lập cấu hình như ảnh -> Save Changes

![cloudwatch](/images/5.sap/012-sap.png)

5. Sau khi cấu hình xong nếu muốn kiểm tra hoạt động 

+ Truy cập vào **CloudTrail** ở thanh task bên trái chọn **Event History**
![cloudtrail](/images/5.sap/013-sap.png)
+ Sau đó chọn các tab như sau để xem hoạt động

![cloudtrail](/images/5.sap/014-sap.png)

6. Kiểm tra chi tiết các log gửi đến CloudWatch từ CloudTrail

Vào giao diện **CloudWatch** chọn **Log Group** -> chọn **Log Group đã tạo** -> vào **log stream** để xem chi tiết.
![cloudwatch](/images/5.sap/015-sap.png)

7. Đến với bước xem chi phí sử dụng 
Ở **AWS Console** search **Billing and Cost Management home**
![Bill](/images/5.sap/016-sap.png)

Ở thanh task bên trái chọn mục **Bill**
![Bill](/images/5.sap/017-sap.png)

Kéo và tìm mục **Charge by Service**
Sẽ thấy các tài nguyên đã được sử dụng và đã được AWS tính phí sử dụng
![Bill](/images/5.sap/018-sap.png)