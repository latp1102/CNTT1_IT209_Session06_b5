# Bài 5 - Thiết kế và Cấu hình dịch vụ Systemd Service cho ứng dụng Java

## 1. Mục tiêu

- Thiết kế Systemd Service để hệ điều hành quản lý vòng đời ứng dụng.
- Chạy ứng dụng dưới user giới hạn `java-runner`.
- Cấu hình tự động restart khi tiến trình gặp lỗi.

## 2. Tạo user hệ thống

Lệnh sử dụng:

```bash
sudo useradd -r -s /usr/sbin/nologin java-runner
