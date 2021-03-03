# Cài đặt ZendServer trên CentOS7

## Yêu cầu

- Đăng nhập quản trị vào máy chủ (root / sudo)

- Truy cập Internet để tải xuống các tài nguyên để cài đặt (ví dụ: Download.zend.com, kho lưu trữ phân phối của bạn cho các phần phụ thuộc, nginx.org nếu bạn sử dụng NginX, v.v.).

- Ít nhất 1GB dung lượng đĩa trên điểm gắn kết sẽ được sử dụng cho / usr / local / zend (khoảng 500MB được sử dụng để cài đặt tiêu chuẩn)

## Cài đặt Zend

**Muốn cài version theo tùy chọn vào: http://repos.zend.com/zend-server/**

- Tạo repo cho Zend (version 2019.0)

`vim /etc/yum.repo.d/zend.repo`

Thêm cấu hình vào zend.repo

```
[Zend]
name=zend-server
baseurl=http://repos.zend.com/zend-server/2019.0/rpm_apache2.4/$basearch
enabled=1
gpgcheck=1
gpgkey=http://repos.zend.com/zend.key

[Zend_noarch]
name=zend-server - noarch
baseurl=http://repos.zend.com/zend-server/2019.0/rpm_apache2.4/noarch
enabled=1
gpgcheck=1
gpgkey=http://repos.zend.com/zend.key

```
- Cài đặt:

For Apache: 

`yum install zend-server`

For Apache-FPM: 

`yum install zend-server-apache-fpm`

For NginX: 

`yum install zend-server-nginx`

- Sau khi cài đặt kiểm tra

`yum clean all`

Truy cập địa chỉ IP với port 10081

`http://<Server_IP>:10081/ZendServer`







## Tài liệu



https://help.zend.com/zend/current/content/rpm_installing_zend_server.htm

https://help.zend.com/zend/zend-server-8/content/rpm_installing_zend_server.htm

http://repos.zend.com/zend-server/

https://www.digitalocean.com/community/tutorials/how-to-install-zend-server-6-on-a-centos-6-4-vps#reference-paths-and-files
