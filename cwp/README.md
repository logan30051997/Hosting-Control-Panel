# Hướng dẫn cài đặt CWP trên CentOS7

## Yêu cầu cấu hình

- Chỉ cài đặt CWP trên máy chủ CentOS 7 mới được cài đặt mà không có bất kỳ thay đổi cấu hình nào.

- Yêu cầu RAM tối thiểu cho 32-bit 512MB và 64-bit 1GB với 10GB dung lượng trống.

- Hiện chỉ hỗ trợ địa chỉ IP tĩnh, không hỗ trợ địa chỉ IP động, cố định hoặc nội bộ.

- Không có bất kỳ trình gỡ cài đặt nào để xóa CWP sau khi cài đặt, bạn phải tải lại hệ điều hành để xóa nó.

## Set ip tĩnh và Set hostname server CentOSS7

## Download và cài đặt CWP

```
# yum -y update
# yum -y install wget
# cd /usr/local/src
# wget http://centos-webpanel.com/cwp-el7-latest
# sh cwp-el7-latest
```


## Tài liệu tham khảo

https://www.tecmint.com/install-centos-web-panel-on-centos-7/

