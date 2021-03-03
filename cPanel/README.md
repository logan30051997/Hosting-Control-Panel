
## Yêu cầu cài đặt

Yêu cầu cài đặt cPanel
- CentOS 7 VPS
- Tối thiểu 1GB RAM (nên sử dụng RAM 2 GB)
- Dung lượng đĩa tối thiểu 20 GB (khuyến nghị 40 GB)
- Giấy phép cPanel (cũng có thời gian dùng thử 15 ngày được kích hoạt ngay sau khi quá trình cài đặt hoàn tất)

## Cài đặt

- Set hostname cho server

`hostnamectl set-hostname cpanel.linex.com`

- Download và cài đặt WHM/Cpanel

` cd /home && curl -o latest -L https://securedownloads.cpanel.net/latest`

`sh latest`

- Sau khi cài đặt vào địa chỉ ip (domain) của server để kiểm tra

`https: // your-server-ip:2087`

## Tài liệu liên quan:

https://dangkyhosting.com/huong-dan-cai-dat-whm-va-cpanel-tren-centos-7.html

https://www.tecmint.com/install-cpanel-whm-in-centos-7/


https://forums.cpanel.net/threads/your-system-is-missing-the-file-etc-fstab.621043/ 
