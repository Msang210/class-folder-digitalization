# Phase 1: Feature Ideation & Scope Definition

> **Dự án:** Digital Class Folder (DCF)  
> **Domain:** EdTech — Trung tâm Tiếng Anh  
> **Ngày:** 2026-05-30  
> **Tác giả:** BA Team  

---

## 1. Bối cảnh hiện trạng (As-Is)

| Hạng mục | Hiện trạng (Sổ tay) | Vấn đề |
|---|---|---|
| **Ghi nhận xét hàng ngày** | TA viết tay vào sổ CF, mỗi ngày chọn 5 học viên bất kỳ | Tốn thời gian, chữ xấu khó đọc, không biết ai đã/chưa được nhận xét |
| **Báo cáo định kỳ (Tuần 5, 10)** | TA viết báo cáo tổng hợp bằng tay | Khó tổng hợp từ các ghi chú rời rạc, thiếu data lịch sử |
| **Chuyển giao cho ASA** | ASA nhận sổ vật lý, đọc → gọi điện/nhắn tin phụ huynh | Chậm trễ, dễ sót thông tin, không track được đã liên hệ PH nào |
| **Lưu trữ** | Sổ giấy xếp chồng cuối khóa | Mất sổ = mất data, không tra cứu được lịch sử |

---

## 2. Đề xuất tính năng sáng tạo (5 tính năng cốt lõi)

### Tính năng 1: Auto-Rotate & Suggestion Engine (Gợi ý học viên hàng ngày)

**Mô tả:** Thay vì TA tự nhớ phải nhận xét ai, hệ thống sẽ tự động gợi ý 5 học viên cần được nhận xét hôm nay. Thuật toán ưu tiên:
- Học viên **chưa được nhận xét lâu nhất** trong tháng
- Học viên có **dấu hiệu cần theo dõi sát** (nhiều tag tiêu cực gần đây)
- Đảm bảo **phân bổ đều** — mỗi học viên được nhận xét ít nhất X lần/tháng

**Giá trị:** TA không phải tự nhớ, không bỏ sót học viên nào. Mọi em đều được "chăm sóc" công bằng. Đảm bảo đến cuối khóa, số lượng nhận xét của mọi học viên đều đồng đều.

---

### Tính năng 2: Quick Tags & Snippets (Nhập liệu siêu tốc)

**Mô tả:** Thay vì gõ tay từng câu, TA chỉ cần tap/click vào các thẻ có sẵn (Quick Tags) được chia theo nhóm: Thái độ, Kỹ năng, Bài tập.
- Ví dụ: `#ThiếuBàiTập`, `#HăngHái`, `#MấtTậpTrung`, `#Phát_âm_tốt`.
- Hệ thống hỗ trợ sinh các câu nhận xét mẫu hoàn chỉnh (Snippets) từ những thẻ này để TA chọn nhanh.

**Giá trị:** Giảm 70-80% thời gian nhập liệu. Đồng nhất tone/chất lượng nhận xét giữa các TA thay vì gõ text dài.

---

### Tính năng 3: Real-time Incident Alert (Cảnh báo sự cố tức thời)

**Mô tả:** Khi có sự cố trong lớp (học sinh xô xát, bị bệnh, vắng không phép...), TA có thể chọn tag sự cố (VD: `#XôXát`, `#Bệnh`) hoặc cắm cờ "Urgent".
- Hệ thống lập tức push notification/email đến ASA phụ trách ngay tại thời điểm đó thay vì đợi TA nộp sổ cuối giờ.

**Giá trị:** Đảm bảo ASA nhận thông tin theo thời gian thực (real-time) để xử lý tức thời, nâng cao trải nghiệm phụ huynh và xử lý rủi ro kịp thời.

---

### Tính năng 4: Auto-Draft Periodic Reports (Tự động tổng hợp báo cáo Tuần 5/10)

**Mô tả:** Đến tuần 5 và tuần 10, hệ thống tự động:
1. **Tổng hợp** tất cả nhận xét hàng ngày + checklist BTVN → "Nháp" sẵn vào form báo cáo (Pre-fill).
2. TA chỉ cần **review, tinh chỉnh, bổ sung nhận xét tổng quan** → Submit.

**Giá trị:** Trước đây TA mất 30-45 phút/báo cáo/lớp. Giờ chỉ còn 5-10 phút review. Data nhất quán, không bỏ sót.

---

### Tính năng 5: ASA Communication Dashboard

**Mô tả:** Màn hình dành riêng cho ASA, gom nhóm các học viên "Cần chú ý" (At-risk students) hiển thị theo dạng timeline:
- **Danh sách báo cáo mới / Alert sự cố** cần xử lý.
- Nút **`Generate Message Template`** để tự động tạo mẫu tin nhắn Zalo/Email chuẩn format (dựa trên data TA đã nhập) để ASA copy-paste gửi thẳng cho phụ huynh.
- **Trạng thái liên hệ PH**: Chưa liên hệ / Đã gọi / Đã gửi tin / PH đã phản hồi.

**Giá trị:** ASA không bị "rơi rớt" thông tin. Rút ngắn thời gian soạn tin nhắn, tăng tốc độ phản hồi phụ huynh.

---

## 3. Danh sách Core Features thiết yếu cho MVP

Dựa trên phân tích **Impact (tác động) × Effort (công sức)**, danh sách MVP (Minimum Viable Product) được đề xuất bao gồm:

### Ma trận ưu tiên tính năng (Impact x Effort Matrix)

| Tính năng | Impact (Tác động) | Effort (Công sức) | Nhóm |
|---|---|---|---|
| Quick Tags | Rất Cao | Thấp | **Quick Win** — MVP |
| Auto-Rotate | Cao | Trung bình | **Quick Win** — MVP |
| Auto-draft Report | Cao | Thấp | **Quick Win** — MVP |
| TQM Dashboard | Cao | Trung bình | **Major Project** — MVP |
| Real-time Alert | Rất Cao | Cao | **Major Project** — MVP |
| Parent Portal | Rất Cao | Rất Cao | **Major Project** — Post-MVP |
| AI Comment Gen | Trung bình | Rất Cao | **Thankless Task** — Post-MVP |

### MVP — Core Features (Phải có)

| # | Tính năng | Lý do "Must-have" |
|---|---|---|
| F1 | **Dashboard TA** — Xem lớp học, danh sách học viên, lịch dạy | Entry point của toàn bộ hệ thống |
| F2 | **Auto-Rotate & Suggestion Engine** — Gợi ý 5 học viên cần nhận xét | Giải quyết pain point "không biết chọn ai", đảm bảo công bằng |
| F3 | **Daily Comment Form (Quick Tags)** — Nhập nhận xét bằng tag siêu tốc | Core workflow — giảm thiểu gõ text dài |
| F4 | **Real-time Incident Alert** — Cảnh báo sự cố tức thời cho ASA | Giúp xử lý khủng hoảng / sự cố khẩn kịp thời |
| F5 | **Auto-Draft Periodic Reports** — Báo cáo định kỳ tuần 5 & 10 | Giải quyết pain "tổng hợp mất thời gian" |
| F6 | **ASA Communication Dashboard** — Xử lý báo cáo, track trạng thái | Hoàn thiện luồng end-to-end: TA → System → ASA → PH |

### Post-MVP — Nice to Have (Phase 2+)

| # | Tính năng | Ghi chú |
|---|---|---|
| F7 | AI-Powered Auto-Generate Comment | Tự động sinh văn bản mềm mại từ các Tag bằng AI |
| F8 | Student Progress Tracker (Biểu đồ) | Cần tích lũy data ít nhất 1-2 khóa mới có ý nghĩa |
| F9 | Parent Portal / Báo cáo trực tuyến cho PH | Mở rộng scope lớn, xem xét ở phase tiếp theo |

---

## 4. Actors & Roles trong hệ thống

| Actor | Vai trò | Tương tác chính |
|---|---|---|
| **TA (Teaching Assistant)** | Người nhập liệu chính | Nhận xét hàng ngày, tick BTVN, cảnh báo sự cố, báo cáo định kỳ |
| **ASA (Academic Support Assistant)** | Người tiếp nhận & truyền đạt | Nhận báo cáo/cảnh báo, tạo template tin nhắn, liên hệ phụ huynh |
| **Giáo viên (Teacher)** | Người dùng phụ | Xem thông tin lớp, thêm ghi chú phụ (Teacher note) |
| **Hệ thống (DCF Platform)** | Xử lý tự động | Suggest học viên, pre-fill báo cáo, push alert, lưu trữ |
| **TQM / Academic Manager** | Quản lý & giám sát | Xem Dashboard SLA, audit chất lượng CF, lấy mẫu ngẫu nhiên |
| **Phụ huynh** *(post-MVP)* | Nhận thông tin | Xem báo cáo online (nếu có Parent Portal) |
