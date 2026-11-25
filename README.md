# Chuyện Thương Hiệu Production

Skill tiếng Việt cho toàn bộ quy trình **tìm tin → kiểm chứng → hook → kịch bản Vbee → MP3 → tự tìm clip → dựng video → QA → caption Facebook**.

Dành cho nội dung thương hiệu, kinh tế, AI, lương, nhân sự và gia đình, hướng tới người xem Việt Nam 25–54 tuổi. Tổng hợp các lựa chọn trực tiếp của chủ kênh đến **25/11/2026**.

## Tải gói skill

**[Tải chuyen-thuong-hieu-production.zip](chuyen-thuong-hieu-production.zip)**

Đọc nhanh toàn bộ quy tắc trong **[SKILL.md](SKILL.md)**. File ZIP chứa một thư mục skill hoàn chỉnh với hướng dẫn, script và tài nguyên.

Giải nén, đặt thư mục `chuyen-thuong-hieu-production` vào thư mục skills của công cụ đang dùng; với Codex cá nhân thường là `~/.codex/skills/`. Gọi skill bằng `$chuyen-thuong-hieu-production` hoặc cung cấp file SKILL.md cho trợ lý hỗ trợ Agent Skills.

Ví dụ: “Dùng $chuyen-thuong-hieu-production để dựng video từ MP3 này, tự tìm clip và kiểm tra bản xuất.”

## Những lựa chọn đã được lưu

- Hook có thương hiệu, cụ thể, đọc một lần hiểu ngay; thu hút bằng dữ kiện.
- Sau hook vào thẳng diễn biến chính, không đọc tên báo hoặc giờ đưa tin.
- Vbee HN – Ngọc Huyền 1.1x, phiên âm tên và break đúng nhịp.
- Khung cam đỏ chỉ ở hook, title trắng căn trái; thân giữ hình ngang sắc nét đủ chiều rộng, nền mờ trên/dưới và logo góc phải.
- **Mỗi cảnh giữ ít nhất hết một câu**, tính cả điểm cắt sẵn trong clip nguồn.
- Karaoke căn theo âm thanh, nằm trong safe area; bỏ ô thông tin và nhãn nhỏ đè lên hình.
- Nhạc cao trào từ 00:48,08 của bản Blockbuster Trailer chủ kênh cung cấp, gain −20 dB, chạy xuyên suốt.
- Đo/soát chính MP4 sau khi xuất và bàn giao file thật.

## Trong gói

```text
chuyen-thuong-hieu-production/
├── SKILL.md
├── agents/openai.yaml
├── assets/                 Khung, logo, safe area và thông số/phiên âm
├── references/rendering.md
├── scripts/                ASR, căn từ, dựng và kiểm tra MP4
└── requirements.txt
```

Chuẩn bị MP3, tư liệu có nguồn, font đủ dấu Việt và đúng bản nhạc nền đang dùng. File nhạc ngoài được khai báo bằng `music.path`; gói public lưu thông số nhạc thay vì phân phối lại file đó. Cách cài thư viện và manifest dựng nằm trong `references/rendering.md` của gói.

Kịch bản được duyệt, file giọng, video và tài khoản của từng dự án được quản lý trong thư mục làm việc riêng. Skill sử dụng khung/logo Chuyện Thương Hiệu đi kèm; public repository không tự cấp giấy phép đối với tư liệu bên thứ ba.
