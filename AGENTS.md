# AGENTS.md: Đảo Đèn Lồng - Phase 1

Dự án game 3D góc nhìn thứ ba, thực hiện theo quy trình AI SDLC 4 phase.
Tác giả: Phạm Ngọc Trung Quân (MSSV: 2A202603626, Lớp K5-L3A).

## Quy ước & lệnh
- Cài đặt: `npm ci`
- Test tự động: `npm test`
- Chạy headless: `node src/headless.js --seed 1 --night 1 --ticks 600 --out out.jsonl`
- Chạy giao diện dev: `npm run dev`
- Build sản phẩm: `npm run build`

## Nguyên tắc Phase 1
- Tuyệt đối tách riêng logic mô phỏng (`src/sim`) khỏi phần render (`src/client`) để headless chạy 60 tick/s không phụ thuộc DOM/WebGL.
- Tuân thủ Test Contract v1.0: tính tất định, format JSONL snapshot/event/end chuẩn xác.
