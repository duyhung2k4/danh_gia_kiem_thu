# Phần Mềm Tính Tiền Dạy

## 🧾 Giới thiệu

**Phần mềm tính tiền dạy** là một hệ thống quản lý giúp nhà trường hoặc các tổ chức giáo dục:
- Thiết lập định mức tiền công cho mỗi tiết dạy.
- Áp dụng hệ số cho giáo viên dựa theo bằng cấp, học vị.
- Xác định hệ số cho từng lớp học dựa vào quy mô, cấp học,...
- Tự động tính toán tổng thu nhập giảng dạy của từng giáo viên trong một học kỳ.

## 💡 Mục tiêu
- Hạn chế việc tính toán thủ công gây sai sót.
- Minh bạch, rõ ràng và linh hoạt trong cách xác định mức thu nhập.
- Dễ dàng mở rộng và tích hợp với các hệ thống quản lý trường học khác.

## 🧠 Tính năng chính

### 1. Thiết lập định mức
- Xác định số tiền chuẩn cho một tiết dạy (VD: 50.000đ/tiết).

### 2. Thiết lập hệ số giáo viên
- Gán hệ số cho giáo viên dựa theo bằng cấp như Cử nhân, Thạc sĩ, Tiến sĩ...

### 3. Thiết lập hệ số lớp học
- Thiết lập hệ số lớp dựa trên quy mô, cấp học hoặc các tiêu chí khác.

### 4. Tính toán tiền dạy
- Tổng tiền dạy = Số tiết × Định mức × Hệ số giáo viên × Hệ số lớp.
- Cho phép tính theo từng học kỳ hoặc cả năm.

### 5. Quản lý dữ liệu
- Quản lý danh sách giáo viên, lớp học, môn học và các thông tin liên quan.

## 🏗️ Kiến trúc hệ thống

- **Frontend**: ReactJS, MantineUI
- **Backend**: Golang (Gin Framework), PostgreSQL
- **Hạ tầng**: Docker, AWS, Kubernetes
- **Khác**: RabbitMQ (nếu cần xử lý bất đồng bộ), Prometheus + Grafana (giám sát)

## 📦 Triển khai
```bash
git clone https://gitlab.com/your-org/teaching-salary-calc.git
cd teaching-salary-calc
docker-compose up -d
