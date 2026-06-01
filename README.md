# Digital Class Folder (DCF) - Business Analysis Portfolio

Chào mừng bạn đến với dự án **Số hóa "Sổ Đầu Bài" (Digital Class Folder)** dành cho trung tâm Anh ngữ. Đây là một dự án phân tích nghiệp vụ (Business Analysis) từ giai đoạn lên ý tưởng (Ideation) đến thiết kế giao diện (UI/UX Prototype), thể hiện cách tiếp cận giải quyết một vấn đề vận hành thực tế bằng công nghệ.

---

## 🎯 Tổng quan dự án (Project Overview)

- **Vấn đề cốt lõi:** Việc sử dụng "Sổ Đầu Bài" bằng giấy hoặc Google Sheets phân tán tại các trung tâm tiếng Anh gây tốn thời gian cho Trợ giảng (TA), dẫn đến chậm trễ trong việc cập nhật thông tin cho Phụ huynh và khó khăn trong việc quản lý chất lượng giảng dạy.
- **Giải pháp:** Xây dựng hệ thống **DCF Platform (VUS Portal)** giúp TA nhập liệu nhanh chóng bằng Quick Tags, tự động xoay vòng đánh giá học viên (Auto-Rotate), và gửi cảnh báo tức thời (Real-time Alert) cho bộ phận Hỗ trợ học thuật (ASA) khi có sự cố.
- **Mục tiêu:** Giảm 70% thời gian nhập liệu cho TA, tăng tốc độ xử lý sự cố từ "buổi hôm sau" xuống còn `< 2 giờ`, và tăng tỷ lệ hoàn thành sổ đầu bài lên `> 95%`.

---

## 📂 Cấu trúc Repository

Dự án được cấu trúc theo các Phase phát triển nghiệp vụ, bạn có thể đọc theo thứ tự từ trên xuống dưới để nắm rõ toàn bộ quy trình:

### 1. [Tài liệu Nghiệp vụ (Docs)](docs/)
Chứa các tài liệu phân tích và thiết kế hệ thống chi tiết:
- 📄 [Phase 1: Feature Ideation & Scope](docs/phase1-feature-ideation.md) - Phân tích tính năng, định nghĩa In-Scope/Out-of-Scope và xác định các Actors.
- 📄 [Phase 2: Business Process Flow](docs/phase2-process-flow.md) - Sơ đồ luồng quy trình nghiệp vụ (As-Is & To-Be), BPMN Swimlane.
- 📄 [Phase 3: BRD & User Stories](docs/phase3-brd-user-stories.md) - Tài liệu Yêu cầu Nghiệp vụ (BRD), Use Cases chi tiết và User Stories theo chuẩn INVEST.

### 2. [Sơ đồ (Diagrams)](diagrams/)
*(Lưu ý: Các sơ đồ luồng dữ liệu, BPMN và Sequence Diagram được nhúng trực tiếp dưới dạng mã Mermaid trong các file tài liệu Markdown ở thư mục `docs/`. Bạn có thể sử dụng tính năng Preview của GitHub hoặc các trình biên dịch Markdown để xem trực quan.)*

### 3. [Giao diện (Prototype)](prototype/)
Các thiết kế giao diện mô phỏng (Mockups/Wireframes) được xây dựng dựa trên các User Stories đã định nghĩa:
- 🖼️ **1_ta_dashboard.png:** Màn hình tổng quan của Trợ giảng (TA).
- 🖼️ **2_class_folder_form.png:** Màn hình nhập liệu Sổ đầu bài với tính năng Quick Tags.
- 🖼️ **3_class_monitor.png:** Màn hình theo dõi tiến độ các lớp đang dạy.
- 🖼️ **4_student_profile.png:** Hồ sơ học viên và lịch sử nhận xét.
- 🖼️ **5_asa_dashboard.png:** Màn hình Communication Queue dành cho bộ phận ASA xử lý cảnh báo khẩn cấp.

---

## 🛠️ Các kỹ năng BA nổi bật trong dự án

Dự án này thể hiện năng lực trong các khía cạnh:
1. **Requirements Elicitation & Analysis:** Phân tích từ Pain-points thực tế để đưa ra các tính năng High-Impact (như Quick Tags, Auto-Rotate Suggestion).
2. **Process Modeling:** Lập bản đồ quy trình nghiệp vụ hiện tại (As-Is) và đề xuất quy trình số hóa (To-Be) sử dụng Sequence Diagram.
3. **Documentation:** Viết Business Requirements Document (BRD), Use Case Specifications chi tiết.
4. **Agile Framework:** Chuyển đổi yêu cầu thành các User Stories có thể phát triển được, đảm bảo tiêu chí INVEST và có Acceptance Criteria rõ ràng.
5. **UI/UX Translation:** Khả năng hình dung và truyền đạt yêu cầu hệ thống thành các thiết kế giao diện trực quan và thân thiện với người dùng cuối (TA & ASA).

---

*Cảm ơn bạn đã dành thời gian xem qua dự án này!*
