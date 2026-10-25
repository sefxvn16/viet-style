# viet-style

[English](README.md) | **Tiếng Việt**

Skill cho trợ lý AI quy định ký tự, dấu câu và thể thức trình bày cho văn bản tiếng Việt hoàn thiện. Skill chọn một chuẩn theo loại văn bản: APA 7 cho văn bản học thuật, Nghị định 30/2020/NĐ-CP cho văn bản hành chính và hồ sơ dự án, và bộ quy định chung cho các trường hợp còn lại. Hướng dẫn trong `SKILL.md` viết bằng tiếng Việt.

## Skill làm gì

- **Chọn một chuẩn theo loại văn bản**, không trộn: học thuật (APA 7), hành chính và hồ sơ dự án (Nghị định 30/2020/NĐ-CP), các trường hợp khác (quy định chung).
- **Quy định chung** (V01 đến V04): gạch ngang ngắn thay gạch dài, nháy kép cong, chữ "và" thay "&", không dấu phẩy trước "và". Quy tắc mới thêm bằng một dòng vào bảng.
- **Văn bản hành chính và hồ sơ dự án:** khổ giấy, lề, phông, số ký hiệu, địa danh và ngày tháng, bố cục nội dung, chữ ký, nơi nhận, phụ lục, chữ viết tắt tên loại, mẫu trình bày, viết hoa, bản sao. Phần này nằm trong `references/nghi-dinh-30.md` và chỉ đọc khi soạn loại văn bản đó.
- **Rà trước khi giao:** đọc lại bản nháp theo chuẩn đã chọn và nói rõ đã áp chuẩn nào.

## Ranh giới

- Áp dụng cho văn bản tiếng Việt hoàn thiện người dùng sẽ gửi đi hoặc xuất bản, và văn bản làm trên canvas hoặc artifact.
- **Không** áp dụng cho câu trả lời hội thoại thường trong chat, code, tên biến, lệnh, commit message, văn bản tiếng Anh và phần trích nguyên văn.
- Chỉ lo ký tự, dấu câu và thể thức. Skill không chứa quy tắc văn phong hay phương pháp chuyên môn.

## Cấu trúc thư mục

```
viet-style/
  SKILL.md
  references/
    nghi-dinh-30.md   # Nghị định 30/2020/NĐ-CP: thể thức, mẫu, viết hoa
README.md
README.vi.md
LICENSE.md
```

## Cài đặt

### Ứng dụng Claude (claude.ai, Claude desktop)

1. Tải repo về, nén riêng thư mục `viet-style` thành `viet-style.zip` (file zip phải chứa thư mục `viet-style` ở cấp ngoài cùng, bên trong có `SKILL.md` và `references/`).
2. Mở Claude, vào **Customize → Skills**, bấm **+** → **Create skill** → **Upload a skill** và chọn `viet-style.zip`. Tên và vị trí menu có thể khác tùy phiên bản ứng dụng. Skill cần bật tính năng chạy mã (code execution).
3. Kiểm tra skill `viet-style` đã hiện trong danh sách và đang bật.

### Claude Code

Chép thư mục `viet-style` vào `~/.claude/skills/` (dùng cho mọi dự án) hoặc `.claude/skills/` của một dự án, rồi khởi động lại Claude Code.

## Cách dùng

Skill kích hoạt khi bạn soạn, sửa, rà soát hoặc chuyển đổi một văn bản tiếng Việt hoàn thiện, có hoặc không gõ lệnh. Ví dụ:

- "Soạn công văn gửi Sở Kế hoạch và Đầu tư về việc …"
- "Rà bản thuyết minh dự án này theo thể thức Nghị định 30."

## Giới hạn

- Phần Nghị định 30 được đối chiếu với bản scan văn bản gốc qua OCR. Vị trí các ô thể thức, hai bộ mặc định về lề và cỡ chữ, cách xử lý thuyết minh dự án là suy ra từ sơ đồ, mẫu hoặc thực hành, không phải câu chữ riêng của nghị định.
- Phụ lục IV đến VI của nghị định (sổ đăng ký, hệ thống quản lý) không đưa vào.
- Khi áp APA 7 cho tài liệu và tác giả tiếng Việt, theo hướng dẫn chính thức của APA hoặc quy định của trường, tạp chí nơi nộp bài.
- Việc rà soát làm bằng cách đọc lại, không dùng script.

## Góp ý

Mọi góp ý xin gửi qua mục **Issues** của repo. Nên ghi: loại văn bản, chuẩn bạn mong đợi và kết quả thực tế (đã bỏ thông tin cá nhân hoặc thông tin mật).

## Giấy phép

Skill phát hành theo giấy phép **CC BY-NC 4.0**: dùng miễn phí cho mục đích phi thương mại, cần ghi nguồn. Muốn dùng thương mại, vui lòng liên hệ tác giả qua mục **Issues**. Xem [LICENSE.md](LICENSE.md).
