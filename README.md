# 🏨 HotelLink - Hotel Booking & Management System

<p align="center">
  <b>HotelLink</b> là hệ thống web full-stack mô phỏng quy trình <b>đặt phòng</b>, <b>quản lý lưu trú</b>, <b>thanh toán</b> và <b>vận hành khách sạn</b> trong thực tế.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-Frontend-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Spring%20Boot-Backend-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/MariaDB-Database-003545?style=for-the-badge&logo=mariadb&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-Container-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS%20EC2-Deploy-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
</p>

---

## ✨ Giới thiệu

**HotelLink** là dự án web full-stack được xây dựng nhằm mô phỏng một hệ thống đặt phòng và quản lý khách sạn gần với môi trường thực tế. Dự án hỗ trợ nhiều nhóm người dùng khác nhau như **khách hàng**, **nhân viên khách sạn** và **quản trị viên**, mỗi nhóm có quyền hạn và nghiệp vụ riêng.

Không chỉ dừng lại ở một website đặt phòng đơn giản, HotelLink tập trung mô phỏng toàn bộ vòng đời vận hành khách sạn: từ lúc khách tìm phòng, đặt phòng, thanh toán, nhận email, đến khi nhân viên check-in, check-out, thêm dịch vụ và quản trị viên theo dõi dữ liệu hệ thống.

---

## 🎯 Mục tiêu dự án

HotelLink được xây dựng với mục tiêu giúp người dùng trải nghiệm một quy trình đặt phòng trực tuyến thuận tiện, đồng thời giúp nhân viên và quản trị viên khách sạn quản lý nghiệp vụ hiệu quả hơn. Dự án cũng là cơ hội để thực hành quy trình phát triển một sản phẩm full-stack hoàn chỉnh, có xác thực, phân quyền, thanh toán online, gửi email, quản lý hình ảnh, Docker hóa ứng dụng và triển khai lên server thật.

---

## 🧩 Bài toán HotelLink giải quyết

Trong mô hình vận hành truyền thống, khách sạn thường phải xử lý nhiều công việc rời rạc như nhận đặt phòng qua điện thoại, ghi chú thủ công, cập nhật trạng thái phòng bằng file riêng hoặc xử lý hóa đơn theo cách thiếu đồng bộ.

HotelLink gom các nghiệp vụ đó vào một hệ thống thống nhất, giúp khách hàng có thể chủ động đặt phòng online, nhân viên dễ dàng xử lý quy trình lưu trú, còn quản trị viên có thể kiểm soát dữ liệu nền tảng của khách sạn ở một nơi duy nhất.

---

## 👥 Vai trò người dùng

| Vai trò               | Mục đích sử dụng                       | Quyền thao tác chính                                                |
| --------------------- | -------------------------------------- | ------------------------------------------------------------------- |
| 🧳 **Khách hàng**     | Đặt phòng và sử dụng dịch vụ khách sạn | Tìm phòng, đặt phòng, thanh toán, xem lịch sử, gửi đánh giá         |
| 🛎️ **Nhân viên**     | Xử lý nghiệp vụ vận hành hằng ngày     | Tạo đơn, check-in, check-out, thêm dịch vụ, xem hóa đơn             |
| 🛡️ **Quản trị viên** | Quản lý dữ liệu và cấu hình hệ thống   | Quản lý phòng, loại phòng, nhân viên, khách hàng, dịch vụ, đánh giá |

Việc phân quyền theo vai trò giúp hệ thống có cấu trúc gần với cách một khách sạn thực tế vận hành, thay vì chỉ là một website hiển thị thông tin phòng.

---

## 🚀 Chức năng nổi bật

### 🧳 Khách hàng

| Chức năng           | Mô tả                                                             |
| ------------------- | ----------------------------------------------------------------- |
| Đăng ký / đăng nhập | Hỗ trợ đăng nhập bằng email, mật khẩu và Google OAuth2            |
| Tìm kiếm phòng      | Lọc phòng theo ngày nhận phòng, ngày trả phòng và nhu cầu lưu trú |
| Xem chi tiết phòng  | Hiển thị hình ảnh, tiện nghi, thông tin phòng và giá              |
| Đặt phòng online    | Cho phép khách tạo đơn đặt phòng trực tuyến                       |
| Chọn dịch vụ đi kèm | Khách có thể thêm dịch vụ trong quá trình đặt phòng               |
| Thanh toán online   | Tích hợp VNPay và MoMo ở môi trường sandbox                       |
| Nhận email          | Gửi email liên quan đến tài khoản và đặt phòng                    |
| Lịch sử đặt phòng   | Theo dõi trạng thái đặt phòng và thanh toán                       |
| Đánh giá dịch vụ    | Gửi đánh giá sau khi sử dụng dịch vụ khách sạn                    |

### 🛎️ Nhân viên khách sạn

| Chức năng         | Mô tả                                                  |
| ----------------- | ------------------------------------------------------ |
| Tạo đơn trực tiếp | Nhân viên có thể tạo đơn đặt phòng cho khách tại quầy  |
| Quản lý đặt phòng | Tìm kiếm, lọc và cập nhật trạng thái đơn đặt phòng     |
| Check-in          | Xác nhận khách nhận phòng                              |
| Check-out         | Hoàn tất quá trình lưu trú của khách                   |
| Thêm dịch vụ      | Bổ sung dịch vụ vào đơn đặt phòng đang có              |
| Xem hóa đơn       | Xem trước hóa đơn trước khi hoàn tất thanh toán        |
| Theo dõi phòng    | Kiểm tra tình trạng phòng và thông tin vận hành cơ bản |

### 🛡️ Quản trị viên

| Chức năng          | Mô tả                                                  |
| ------------------ | ------------------------------------------------------ |
| Quản lý phòng      | Quản lý phòng, tầng, giá và trạng thái phòng           |
| Quản lý loại phòng | Cấu hình loại phòng, tiện nghi và loại giường          |
| Quản lý dịch vụ    | Thêm, sửa, xóa các dịch vụ đi kèm                      |
| Quản lý nhân viên  | Tạo và kiểm soát tài khoản nhân viên                   |
| Quản lý khách hàng | Theo dõi danh sách khách hàng trong hệ thống           |
| Quản lý đánh giá   | Kiểm soát đánh giá và phản hồi từ khách hàng           |
| Theo dõi dữ liệu   | Xem các thông tin quan trọng phục vụ vận hành hệ thống |

---

## 🌟 Điểm nổi bật của dự án

HotelLink không chỉ là một bài demo CRUD đơn giản. Dự án được xây dựng theo hướng mô phỏng một sản phẩm web thực tế với nhiều nghiệp vụ liên kết với nhau.

| Nhóm nổi bật             | Nội dung                                                        |
| ------------------------ | --------------------------------------------------------------- |
| 🔐 Xác thực & phân quyền | Đăng nhập, Google OAuth2, JWT và phân quyền theo vai trò        |
| 🏨 Nghiệp vụ khách sạn   | Đặt phòng, thêm dịch vụ, check-in, check-out và hóa đơn         |
| 💳 Thanh toán            | Tích hợp VNPay và MoMo sandbox để mô phỏng thanh toán online    |
| 📧 Email                 | Gửi email cho các luồng tài khoản và đặt phòng                  |
| ☁️ Lưu trữ ảnh           | Sử dụng Cloudinary để quản lý hình ảnh phòng                    |
| 🐳 Docker hóa            | Đóng gói backend, frontend và database bằng Docker              |
| ⚙️ CI/CD                 | Tự động build, push image và deploy bằng GitHub Actions         |
| 🌐 Deploy thực tế        | Triển khai thử nghiệm lên AWS EC2 để kiểm tra khả năng vận hành |

---

## 🛠️ Công nghệ sử dụng

### Frontend

| Công nghệ            | Vai trò trong dự án                                      |
| -------------------- | -------------------------------------------------------- |
| ⚛️ **React**         | Xây dựng giao diện người dùng dạng component             |
| ⚡ **Vite**           | Tăng tốc quá trình phát triển và build frontend          |
| 🧠 **Redux Toolkit** | Quản lý trạng thái đăng nhập và dữ liệu dùng chung       |
| 🧭 **React Router**  | Điều hướng giữa các trang trong ứng dụng                 |
| 🎨 **Tailwind CSS**  | Xây dựng giao diện responsive, gọn và dễ tùy biến        |
| 🧱 **Shadcn UI**     | Tạo các component UI hiện đại, đồng bộ và dễ tái sử dụng |

### Backend

| Công nghệ                           | Vai trò trong dự án                    |
| ----------------------------------- | -------------------------------------- |
| ☕ **Java 21**                       | Ngôn ngữ chính cho backend             |
| 🍃 **Spring Boot**                  | Xây dựng REST API và xử lý nghiệp vụ   |
| 🛡️ **Spring Security**             | Bảo vệ API và kiểm soát quyền truy cập |
| 🔑 **JWT**                          | Xác thực người dùng bằng token         |
| 🗃️ **Spring Data JPA / Hibernate** | Làm việc với database thông qua ORM    |
| 🔐 **OAuth2**                       | Tích hợp đăng nhập bằng Google         |
| 📩 **Spring Mail**                  | Gửi email cho các nghiệp vụ liên quan  |
| 🔗 **OpenFeign**                    | Kết nối đến dịch vụ bên ngoài như MoMo |

### Database & External Services

| Công nghệ / Dịch vụ   | Vai trò trong dự án                                                  |
| --------------------- | -------------------------------------------------------------------- |
| 🐬 **MariaDB**        | Lưu trữ dữ liệu người dùng, phòng, đặt phòng, thanh toán và danh mục |
| ☁️ **Cloudinary**     | Lưu trữ và quản lý hình ảnh                                          |
| 💳 **VNPay Sandbox**  | Mô phỏng thanh toán qua VNPay                                        |
| 💰 **MoMo Sandbox**   | Mô phỏng thanh toán qua MoMo                                         |
| 🔐 **Google Console** | Cấu hình Google OAuth2                                               |

### DevOps & Deployment

| Công nghệ             | Vai trò trong dự án                               |
| --------------------- | ------------------------------------------------- |
| 🐳 **Docker**         | Đóng gói ứng dụng thành container                 |
| 📦 **Docker Hub**     | Lưu trữ Docker image backend và frontend          |
| ⚙️ **GitHub Actions** | Tự động hóa quy trình build và deploy             |
| ☁️ **AWS EC2**        | Server demo để kiểm thử ứng dụng trên Internet    |
| 🌐 **Nginx**          | Phục vụ frontend và điều hướng request khi deploy |

---

## 🏗️ Kiến trúc tổng quan

<p align="center">
  <img src="https://res.cloudinary.com/dcwauocnz/image/upload/v1779334212/ArchitectureDiagram_ouuggn.png" alt="Architecture Diagram" width="90%" />
</p>

Backend còn kết nối với các dịch vụ bên ngoài như **Google OAuth2**, **VNPay**, **MoMo**, **Cloudinary** và **SMTP Email Service** để hoàn thiện các nghiệp vụ cần thiết.

---

## 🔄 Luồng hoạt động cơ bản

```text
Người dùng
   │
   ▼
Thao tác trên giao diện React
   │
   ▼
Frontend gửi request đến Spring Boot API
   │
   ▼
Backend xác thực JWT và kiểm tra quyền truy cập
   │
   ▼
Backend xử lý nghiệp vụ đặt phòng / thanh toán / check-in / check-out
   │
   ▼
MariaDB lưu trữ và cập nhật dữ liệu
   │
   ▼
Backend gọi dịch vụ ngoài nếu cần: Google, VNPay, MoMo, Cloudinary, Email
   │
   ▼
Frontend nhận response và hiển thị kết quả cho người dùng
```

---

## 🧱 Design Patterns & Code Organization

Trong quá trình phát triển HotelLink, dự án áp dụng nhiều pattern và cách tổ chức code phổ biến để tăng tính rõ ràng, dễ bảo trì và dễ mở rộng.

| Pattern / Kiến trúc              | Cách áp dụng                                                                       |
| -------------------------------- | ---------------------------------------------------------------------------------- |
| **MVC**                          | Tách controller, xử lý nghiệp vụ và dữ liệu trả về                                 |
| **Layered Architecture**         | Chia backend thành controller, service, repository, DTO và config                  |
| **Repository Pattern**           | Tách logic truy vấn database khỏi logic nghiệp vụ                                  |
| **Service Pattern**              | Gom các nghiệp vụ như đặt phòng, thanh toán, check-in, check-out vào service riêng |
| **DTO Pattern**                  | Kiểm soát dữ liệu request / response, tránh trả trực tiếp entity                   |
| **Dependency Injection**         | Dùng Spring Boot quản lý dependency giữa các component                             |
| **Component-Based Architecture** | Chia UI React thành nhiều component nhỏ, dễ tái sử dụng                            |
| **Redux Pattern**                | Quản lý trạng thái đăng nhập, người dùng và dữ liệu dùng chung ở frontend          |

---

## 📁 Cấu trúc thư mục

```text
HotelLink/
├── backend/                    # Mã nguồn backend Spring Boot
│   ├── src/                    # Controller, service, repository, security, config
│   ├── scripts/                # Dữ liệu mẫu và script liên quan
│   └── Dockerfile              # Cấu hình đóng gói backend
│
├── frontend/                   # Mã nguồn frontend React
│   ├── src/                    # Components, pages, layouts, hooks, store
│   ├── public/                 # Tài nguyên tĩnh
│   ├── nginx.conf              # Cấu hình Nginx khi deploy frontend
│   └── Dockerfile              # Cấu hình đóng gói frontend
│
├── .github/workflows/          # Cấu hình GitHub Actions CI/CD
├── docker-compose.yml          # Cấu hình chạy tổng hợp cho dự án
├── docker-compose.prod.yml     # Cấu hình triển khai production/demo
└── README.md                   # Tài liệu giới thiệu dự án
```

---

## ⚙️ CI/CD & Triển khai

HotelLink đã được triển khai thử nghiệm lên **AWS EC2** để kiểm tra khả năng vận hành trên môi trường Internet. Quy trình triển khai bao gồm cấu hình biến môi trường, build ứng dụng, chạy database, kết nối backend với frontend và kiểm tra hoạt động của hệ thống sau khi deploy.

Pipeline CI/CD được xây dựng bằng **GitHub Actions** với mô hình triển khai tự động:

<p align="center">
  <img src="https://res.cloudinary.com/dcwauocnz/image/upload/v1779334221/DeploymentDiagram_jtchle.png" alt="Deployment & CI/CD Diagram" width="90%" />
</p>

Hiện tại server EC2 không được duy trì online liên tục để tránh phát sinh chi phí. Phần deploy được thực hiện với mục đích học tập, demo, kiểm chứng khả năng vận hành thực tế và tích lũy kinh nghiệm DevOps cơ bản.

---

## 📌 Ghi chú

* Dự án được xây dựng với mục đích học tập, thực hành full-stack và mô phỏng quy trình làm sản phẩm gần với thực tế.
* VNPay và MoMo đang sử dụng môi trường sandbox, phù hợp cho demo và kiểm thử.
* Server EC2 có thể không chạy liên tục do giới hạn chi phí vận hành.
* README này tập trung giới thiệu giá trị sản phẩm, kiến trúc, chức năng chính và những phần đã thực hiện.

---

## 👨‍💻 Tác giả

**Phạm Thành Trí**
Software Engineer / Full-stack Developer

---

<p align="center">
  <b>HotelLink</b> - Full-stack hotel booking and management system built with real-world workflow simulation.
</p>
