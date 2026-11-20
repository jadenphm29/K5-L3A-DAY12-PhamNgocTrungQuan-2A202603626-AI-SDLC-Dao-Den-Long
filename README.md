# Đảo Đèn Lồng — Phase 1

Học viên: **Phạm Ngọc Trung Quân** — MSSV: **2A202603626** — Lớp: **K5-L3A**
Dự án game 3D góc nhìn thứ ba áp dụng quy trình AI SDLC.

## Trạng thái Phase 1 (PRD-0, Contract v1.0)
- Hoàn thành Đêm 1 trên Đảo Bến: 5 Đèn Lồng Lớn, đom đóm, Bóng Mực, Tỏa Sáng, tính điểm.
- Chế độ headless theo Test Contract v1.0 đạt 100% tiêu chí tất định và định dạng output JSONL.
- Điều khiển: W A S D di chuyển, Space nhảy, F Tỏa Sáng, E nạp ánh sáng.

## Cài đặt và kiểm thử
```bash
npm ci
npm test
node src/headless.js --seed 1 --night 1 --ticks 600 --out out.jsonl
```
