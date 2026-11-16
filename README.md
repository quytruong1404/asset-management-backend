# ⚙️ ASSET MANAGEMENT SYSTEM - BACKEND REST API

> **Hệ Thống Quản Lý Thiết Bị Nội Bộ (Máy Chủ REST API)**  
> **Học phần:** Chuyên Đề 2 (CD2) / Phát Triển Phần Mềm  
> **Công nghệ:** Spring Boot 3 (Java 17), Spring Data JPA, Hibernate, MySQL 8.0 / H2 In-Memory, OpenAPI 3.0 / Swagger UI  
> **Repository Frontend:** [asset-management-frontend](https://github.com/quytruong1404/asset-management-frontend)

---

## 👥 BẢNG PHÂN CHIA NHIỆM VỤ NHÓM 2 NGƯỜI (50% - 50%)

| Thành viên | Phân hệ Backend đảm nhiệm | REST API Endpoints chi tiết |
| :--- | :--- | :--- |
| **Thành viên 1 (Trương Đàm Công Quý)** | **1. Phân hệ Quản Lý Thiết Bị**<br>(`DeviceController`, `DeviceService`, `DeviceRepository`, `Device` Entity) | - `GET /api/devices`: Lấy danh sách thiết bị<br>- `GET /api/devices/{id}`: Chi tiết 1 thiết bị<br>- `POST /api/devices`: Thêm mới thiết bị<br>- `PUT /api/devices/{id}`: Cập nhật thiết bị<br>- `DELETE /api/devices/{id}`: Xóa thiết bị<br>- `GET /api/categories`: Danh mục thiết bị |
| **Thành viên 2** | **2. Phân hệ Quản Lý Mượn Trả**<br>(`BorrowRequestController`, `BorrowRequestService`, `BorrowRequestRepository`, `BorrowRequest` Entity) | - `GET /api/borrow-requests`: Xem danh sách phiếu<br>- `GET /api/borrow-requests/{id}`: Chi tiết phiếu<br>- `POST /api/borrow-requests`: Tạo phiếu mượn mới<br>- `POST /api/borrow-requests/{id}/approval`: Duyệt / Từ chối<br>- `POST /api/borrow-requests/{id}/return`: Xác nhận đã trả<br>- `DELETE /api/borrow-requests/{id}`: Xóa phiếu |

---

## 📡 TÀI LIỆU SWAGGER UI

Sau khi chạy backend, truy cập:
👉 `http://localhost:8080/swagger-ui/index.html` (hoặc link Cloud Render) để kiểm thử trực tiếp các API.

---

## 🚀 HƯỚNG DẪN CHẠY LOCAL

```bash
# Windows PowerShell
.\mvnw.cmd clean spring-boot:run

# Linux / Mac
./mvnw clean spring-boot:run
```
Máy chủ chạy tại: `http://localhost:8080` (hoặc cổng Render `10000`).
