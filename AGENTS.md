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

## Cập nhật Phase 2 (Contract v1.1)
- Hỗ trợ đầy đủ 3 Đêm: Đảo Bến, Đảo Cau (cầu tre, bục nhảy), Đảo Chuông (3 tầng, dốc, gió mạnh).
- Cơ chế mới: Lướt (Dash), Gió Lạc (Drifter), Bùa Gió (Charm), Tạm dừng (Pause).
- Kiểm tra hồi quy: Chạy `scripts/verify.sh` để kiểm tra cả 3 đêm và tính tất định.

## Cập nhật Phase 3 (Contract v1.2) - Change Request
- Luật mới: Đèn cạn dầu (1 đơn vị/s). Bóng Mực hút dầu khi đèn < 30.
- Thắp lại đèn cũ chỉ tốn 5 đom đóm.
- Thắng mới: Sống sót tới bình minh và giữ >= 60% số đèn đang sáng.
- Bảng màu mù màu (Colorblind mode) & tăng sức chứa dần (capacity progression).
- Ghi rõ quyết định trong ADR 0001 và cập nhật CHANGELOG.
