# Prototype — UI/UX Design Rationale

Thư mục này chứa 5 màn hình thiết kế giao diện cho hệ thống **VUS Portal (DCF Platform)**, được xây dựng dựa trên User Stories và Use Cases đã định nghĩa trong [Phase 3](../docs/phase3-brd-user-stories.md).

> **[Xem thiết kế trên Figma →](https://www.figma.com/design/1EEfOhjwVWJFDik4i4u5yf/Digital-CF?node-id=0-1&t=485Qb1yHpVVvYS0m-1)**

---

## Công cụ & Design System

| Hạng mục | Chi tiết |
|---|---|
| **Tool** | Google Stitch (AI-assisted UI generation) |
| **Figma File** | [Digital CF — VUS Portal](https://www.figma.com/design/1EEfOhjwVWJFDik4i4u5yf/Digital-CF?node-id=0-1&t=485Qb1yHpVVvYS0m-1) |
| **Design System** | VUS Elite Portal — xem spec đầy đủ tại [`prototype/design-system.md`](design-system.md) |
| **Heading Font** | Bricolage Grotesque (Bold 700) |
| **Body Font** | Inter (Regular 400) |
| **Sidebar** | `#1e293b` dark navy, fixed 260px |
| **Primary** | `#1d3072` navy |
| **Urgent/Destructive** | `#e51f08` red (intentional — urgency signal) |
| **Background** | `#f8fafc` off-white |
| **Card Surface** | `#ffffff` white, 8px border-radius, ambient shadow |

---

## Danh sách màn hình

| File | Màn hình | Actor | User Story liên quan |
|---|---|---|---|
| `1_ta_dashboard.png` | TA Dashboard | Teaching Assistant | US-01 (Auto-Rotate) |
| `2_class_folder_form.png` | Class Folder Form | Teaching Assistant | US-01, US-02 (Quick Tags), US-03 (Urgent Alert) |
| `3_class_monitor.png` | Class Monitor | Teaching Assistant | UC-CF-01 (xem tổng quan lớp) |
| `4_student_profile.png` | Student Profile | Teaching Assistant | UC-CF-03 (lịch sử nhận xét) |
| `5_asa_dashboard.png` | ASA Communication Dashboard | ASA | US-04 (Communication Queue) |

---

## Quyết định thiết kế quan trọng

### 1. Quick Tags thay vì textarea tự gõ
Tính năng cốt lõi giảm thời gian nhập liệu. Tag chips màu **xanh lá** = điểm tích cực, **amber** = cần cải thiện — màu sắc có ngữ nghĩa rõ ràng, không cần đọc label.


### 2. Urgent toggle ON state — intentional red
Khi TA bật toggle "Báo cáo sự cố khẩn cấp", toàn bộ card chuyển đỏ, mở text field mô tả và nút "Gửi Alert". Màu đỏ ở đây là **tín hiệu khẩn cấp có chủ đích** — không phải lỗi UI.

### 3. ASA Queue layout (CRM pattern)
Màn hình ASA dùng layout queue (trái) + template preview (phải) theo pattern CRM/helpdesk chuẩn, phân cấp KHẨN CẤP (red border) vs bình thường (blue border) — giúp ASA scan nhanh và ưu tiên xử lý.
