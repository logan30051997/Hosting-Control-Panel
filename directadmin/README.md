# Hướng dẫn cài đặt DirectAdmin

## Yêu cầu

- OS	Version

CloudLinux	6.x 64-bit, 7.x 64-bit, 8.x 64-bit

AlmaLinux / RHEL / CentOS	**7.**x 64-bit, 8.x 64-bit

Debian	8.x 64-bit, 9.x 64-bit, 10.x 64-bit, 11.x 64-bit ALPHA

Ubuntu	16.04 64-bit, 18.04 64-bit, 20.04 64-bit

FreeBSD	11.x 64-bit, 12.x 64-bit

- Resoures

/boot	500 MB

swap	For < 2GB of RAM: 2 x RAM, for 2GB - 8GB of RAM: equal to the amount of RAM, for > 8GB of RAM: at least 4GB

/tmp 1 GB. Highly recommended to mount /tmp with noexec,nosuid in /etc/fstab	

/	6 - 10 GB

/var	8 - 20 GB. Logs, and Databases with CentOS

/usr	5 - 12+ GB. DA data, source code, mysql backups with custombuild option

/home	Rest of drive. Roughly 80% for User data. Mount with nosuid in /etc/fstab if possible.

- Package

```
yum install wget tar gcc gcc-c++ flex bison make bind bind-libs bind-utils openssl openssl-devel perl quota libaio \
libcom_err-devel libcurl-devel gd zlib-devel zip unzip libcap-devel cronie bzip2 cyrus-sasl-devel perl-ExtUtils-Embed \
autoconf automake libtool which patch mailx bzip2-devel lsof glibc-headers kernel-devel expat-devel \
psmisc net-tools systemd-devel libdb-devel perl-DBI perl-Perl4-CoreLibs perl-libwww-perl xfsprogs rsyslog logrotate \
crontabs file kernel-headers ipset
```
## Cài đặt

- Tải bản cài tự động DirectAdmin

```
wget http://www.directadmin.com/setup.sh && chmod 755 setup.sh 

./setup.sh

```

- Đến trang yêu cầu nhập ID và License key

Đăng ký 1 tài khoản trên https://www.directadmin.com/ và tạo 1 key trail

- Đến phần Option lựa chọn các gói cài đi kèm, chọn những gói mà bạn mong muốn và Version thích hợp

- Đợi 15-30p tùy từng máy để tiến hành cài đặt

- Cài đặt xong sẽ hiện ra link đăng nhập DirectAdmin:2222 và tài khoản 

# Tài liệu liên quan

https://vdodata.vn/huong-dan-cai-dat-direct-admin/
