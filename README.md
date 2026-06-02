![Status](https://img.shields.io/badge/Status-Completed-brightgreen) ![Type](https://img.shields.io/badge/Type-BA%20Portfolio-blue) ![Domain](https://img.shields.io/badge/Domain-EdTech-orange)

# 🗂️ Class Folder Digitalization

Dự án **Số hóa "Sổ Đầu Bài" (Digital Class Folder)** cho trung tâm Anh ngữ VUS — từ giai đoạn phân tích vấn đề đến thiết kế giao diện hoàn chỉnh, thể hiện quy trình làm việc thực tế của một Business Analyst.

---

## Problem Statement

| | |
|---|---|
| **Vấn đề** | Việc sử dụng "Sổ Đầu Bài" bằng giấy hoặc Google Sheets phân tán tại các trung tâm tiếng Anh gây tốn thời gian cho Trợ giảng (TA - tốn > 15 phút/buổi). Điều này dẫn đến chậm trễ trong việc cập nhật thông tin cho Phụ huynh và khó khăn trong việc quản lý chất lượng giảng dạy. |
| **Giải pháp** | Xây dựng hệ thống **DCF Platform (VUS Portal)** giúp TA nhập liệu nhanh chóng bằng Quick Tags, tự động xoay vòng đánh giá học viên (Auto-Rotate), và gửi cảnh báo tức thời (Real-time Alert) cho bộ phận Hỗ trợ học thuật (ASA) khi có sự cố. |
| **Mục tiêu** | Giảm 70% thời gian nhập liệu cho TA · Tăng tốc độ xử lý sự cố xuống `< 2 giờ` · Tăng tỷ lệ hoàn thành sổ đầu bài lên `> 95%`. |

---

## Scope & Stakeholders

Dự án tập trung vào luồng nghiệp vụ quản lý lớp học hàng ngày và xử lý cảnh báo sự cố. Bao gồm các bên liên quan (Stakeholders) chính:

1. **Teaching Assistant (TA):** Người dùng chính, trực tiếp nhập liệu Sổ đầu bài và theo dõi lớp.
2. **Academic Support Assistant (ASA):** Tiếp nhận và xử lý các sự cố khẩn cấp (Incident Alert) từ TA.
3. **Teacher (Native/Local):** Xem thông tin lớp học và học viên do TA cập nhật.
4. **TQM / Academic Manager:** Quản lý & giám sát chất lượng vận hành (In-Scope MVP).
5. **Hệ thống (System):** Tự động xử lý Auto-Rotate logic, tính toán SLA và gửi thông báo.

---

## Methodology

Dự án áp dụng các phương pháp phân tích chuẩn trong Business Analysis:
- **Requirements Elicitation:** Áp dụng ma trận Impact × Effort để lọc ra 5 tính năng MVP.
- **Process Modeling:** Lập bản đồ quy trình As-Is (hiện trạng) và To-Be (đề xuất) bằng **BPMN Swimlane** và **Sequence Diagram**.
- **Agile Framework:** Phân rã yêu cầu thành các **Use Case** và **User Stories** theo tiêu chuẩn INVEST. Thiết lập Acceptance Criteria cho 3 kịch bản (happy/edge/negative).
- **UI/UX Prototyping:** Chuyển đổi yêu cầu từ text thành các bản thiết kế giao diện trực quan tuân thủ Design System.

---

## Key Deliverables

Tài liệu được chia thành các Phase rõ ràng, bạn có thể xem chi tiết tại:

- 📄 **[Phase 1 — Feature Ideation & Scope](docs/phase1-feature-ideation.md)**: Phân tích tính năng, định nghĩa In/Out-of-Scope và Actor Table.
- 📄 **[Phase 2 — Business Process Flow](docs/phase2-process-flow.md)**: Sơ đồ BPMN Swimlane, Sequence Diagram và Business Logic. *(Lưu ý: Sơ đồ được nhúng bằng mã Mermaid và tự động render trên GitHub).*
- 📄 **[Phase 3 — BRD & User Stories](docs/phase3-brd-user-stories.md)**: Tài liệu BRD & FRD hoàn chỉnh (Stakeholders, Business Case, Use Cases, User Stories, NFR).

---

## Prototype

5 màn hình thiết kế dựa trên User Stories đã định nghĩa. Design System sử dụng: **Bricolage Grotesque** (heading) + **Inter** (body), sidebar navy `#1e293b`, primary `#1d3072`. Xem tài liệu đặc tả UI tại [`prototype/README.md`](prototype/README.md).

> **[Xem thiết kế tương tác trên Figma →](https://www.figma.com/design/1EEfOhjwVWJFDik4i4u5yf/Digital-CF?node-id=0-1&t=485Qb1yHpVVvYS0m-1)**

### TA Dashboard & Class Folder Form
![TA Dashboard](prototype/1_ta_dashboard.png)
![Class Folder Form](prototype/2_class_folder_form.png)

### Class Monitor & Student Profile
![Class Monitor](prototype/3_class_monitor.png)
![Student Profile](prototype/4_student_profile.png)

### ASA Communication Dashboard
![ASA Dashboard](prototype/5_asa_dashboard.png)

---

## Tools Used

- **Mermaid JS:** Vẽ sơ đồ BPMN, Sequence Diagram trực tiếp bằng code trong Markdown.
- **Google Stitch / Figma:** Lên ý tưởng, xây dựng Design System và thiết kế UI Prototype.
- **Markdown / Git:** Viết tài liệu (Documentation) và quản lý version control.
- **Excel / Google Sheets:** (Giai đoạn As-Is) Công cụ hiện tại đang được sử dụng trước khi số hóa.

---
*Dự án hoàn thành tháng 6/2026.*
