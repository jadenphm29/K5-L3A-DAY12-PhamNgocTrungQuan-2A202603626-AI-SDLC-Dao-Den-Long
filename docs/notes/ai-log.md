# Nhật ký dùng AI (AI Log): Phạm Ngọc Trung Quân (2A202603626)

## Phase 1 (0h - 1h): PRD-0 và Test Contract v1.0
- **Model:** Claude 3.5 Sonnet & Antigravity Lead
- **Công việc:** Phân tích PRD-0, xác lập Test Contract v1.0, thiết kế kiến trúc sim engine tách rời hiển thị, xây dựng headless runner.
- **Lỗi AI gặp phải:** AI ban đầu định nhúng trực tiếp Three.js vào vòng lặp game; đã điều chỉnh tách riêng `src/sim` (logic thuần túy) và `src/client` (render WebGL).
- **Token ước tính:** ~32,000 prompt tokens, ~8,500 completion tokens (~$0.22).
- **Harness:** Tạo `AGENTS.md` v1.0 với các lệnh test và quy ước rõ ràng.
