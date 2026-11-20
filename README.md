# Đảo Đèn Lồng — Phase 3

Học viên: **Phạm Ngọc Trung Quân** — MSSV: **2A202603626** — Lớp: **K5-L3A**
Dự án game 3D góc nhìn thứ ba áp dụng quy trình AI SDLC.

## Trạng thái Phase 3 (Ticket-03 "Đèn cạn dầu", Contract v1.2)
- Cơ chế thay đổi cốt lõi (Change Request):
  + Đèn sáng hao dầu 1.0 fuel/s. Châm dầu bằng tương tác.
  + Đèn < 30 fuel mất vùng an toàn, Bóng Mực wander tìm tới hút dầu (5 fuel/s).
  + Thắp lại đèn đã từng sáng chỉ tốn 5 đom đóm.
  + Điều kiện thắng mới: Giữ >= 60% đèn sáng khi hết giờ bình minh.
  + Sức chứa tăng dần (10 + 2*lần thắp, tối đa 20).
  + Chế độ hiển thị dễ phân biệt cho người mù màu.
- Quyết định kiến trúc: xem [ADR 0001](docs/adr/0001-lantern-fuel-and-dawn-win.md).
- Toàn bộ test cũ được cập nhật có lý do, không bỏ qua test.

## Cài đặt và kiểm thử
```bash
npm ci
npm test
```
