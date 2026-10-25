---
name: viet-style
description: "Quy tắc ký tự, dấu câu và thể thức tiếng Việt theo style cá nhân của người dùng, áp dụng cho văn bản GIAO RA hoặc làm trên canvas/artifact: công văn, tờ trình, hồ sơ dự án, thuyết minh, báo cáo, thư, bài luận, nội dung file Word/Excel/PDF. Văn bản học thuật theo chuẩn APA 7. Văn bản hành chính và hồ sơ dự án theo Nghị định 30/2020/NĐ-CP (thể thức, kỹ thuật trình bày, viết hoa, chữ viết tắt tên loại, mẫu). Trường hợp khác: theo mục Quy định chung của skill (dấu gạch, dấu nháy, chữ “và”…). Kích hoạt mỗi khi soạn, sửa, rà soát hoặc chuyển đổi văn bản tiếng Việt hoàn thiện, kể cả khi người dùng không gõ lệnh và khi văn bản được xuất ra file Word, Excel hoặc PDF. Không áp dụng cho câu trả lời hội thoại thường trong chat, code, tên biến, lệnh, commit message, văn bản tiếng Anh."
---

# viet-style: quy tắc tiếng Việt cá nhân

Skill này chỉ chứa quy tắc về **ký tự, dấu câu và thể thức trình bày**. Không chứa quy tắc văn phong, chống khuôn mẫu AI, hay phương pháp chuyên môn. Skill này độc lập, chỉ gồm văn bản (không có script) và người dùng tự cập nhật khi gặp lỗi mới.

## Phạm vi

- **Áp dụng:** văn bản giao ra (file, nội dung người dùng sẽ gửi đi hoặc xuất bản) và văn bản làm trên canvas/artifact sử dụng tiếng Việt là ngôn ngữ chính.
- **Không áp dụng:**
  - Câu trả lời hội thoại thông thường của AI trong chat (trao đổi, phân tích, giải thích).
  - Code, tên biến, đường dẫn, lệnh, commit message.
  - **Tiếng Anh:** văn bản tiếng Anh và đoạn tiếng Anh xen trong văn bản tiếng Việt giữ nguyên, kể cả dấu gạch và dấu nháy.
  - **Trích nguyên văn:** phần trích đúng từng chữ từ một nguồn (câu trích, tên tài liệu, tên riêng, điều khoản gốc) giữ nguyên ký tự của nguồn.

## Chọn chuẩn theo loại văn bản

Xác định loại văn bản trước, rồi áp đúng một chuẩn. Không trộn.

| Loại văn bản                                                                                                      | Chuẩn áp dụng                                                                                                                    |
| ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| Học thuật (bài luận, bài báo, đề tài, luận văn, case study, bài thi có trích dẫn nguồn)                           | **APA 7**. Mọi thứ theo APA 7, không áp mục Quy định chung.                                                                      |
| Hành chính (quyết định, công văn, tờ trình, thông báo, biên bản, báo cáo gửi cơ quan nhà nước) và **hồ sơ dự án** | **Nghị định 30/2020/NĐ-CP, Phụ lục I** (thể thức, kỹ thuật trình bày; đọc `references/nghi-dinh-30.md`). Chỗ nghị định không quy định thì dùng mục Quy định chung. |
| Các trường hợp khác (thư, báo cáo nội bộ, nội dung website, văn bản thông thường)                                 | Mục **Quy định chung** bên dưới.                                                                                                 |

Chưa rõ loại văn bản mà nó làm đổi cách trình bày: hỏi một câu ngắn, hoặc nêu chuẩn đã chọn khi giao.

Khi quy tắc ở đây xung đột với yêu cầu rõ ràng của người dùng trong lượt hiện tại, làm theo yêu cầu hiện tại và nói rõ chỗ đã khác quy tắc.

## Quy định chung

Đây là nơi duy nhất chứa các quy tắc chung về ký tự, dấu câu, cách viết. Các mục khác chỉ dẫn chiếu tới mục này (không nêu mã V), nên **thêm hoặc sửa quy tắc chỉ cần làm ở bảng dưới**. Áp dụng cho văn bản tiếng Việt thuộc nhóm "khác" và cho chỗ Nghị định 30 không quy định. Thêm quy tắc mới ở cuối bảng, không đánh số lại.

| Mã  | Quy tắc                          | Dùng                                         | Không dùng                                                                                                  | Lý do / ghi chú                                                                                                                                                                             |
| --- | -------------------------------- | -------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| V01 | Dấu gạch ngang và dấu nối        | Gạch ngang ngắn `-` (U+002D)                 | Em dash `—` (U+2014), en dash `–` (U+2013), dấu trừ `−` (U+2212), các gạch Unicode khác (U+2010 đến U+2015) | Người Việt không dùng gạch dài trong hồ sơ, văn bản. Áp dụng cho mọi vai trò: ngăn cách ý, khoảng số, ngày, dấu nối, tên ghép.                                                              |
| V02 | Dấu trích dẫn và đánh dấu từ ngữ | Nháy kép cong `“…”` (U+201C mở, U+201D đóng) | Nháy kép thẳng `"…"` (U+0022), nháy đơn `'…'`                                                               | Chuẩn trong hồ sơ, văn bản, báo cáo tiếng Việt.                                                                                                                                             |
| V03 | Liên từ "và"                     | Chữ "và"                                     | Ký hiệu `&`                                                                                                 | Dùng chữ "và" trong phần tiếng Việt: "Nguyễn Văn A và Trần Thị B", "Sở Kế hoạch và Đầu tư". Tên riêng tiếng Anh có sẵn `&` (ví dụ tên công ty nước ngoài) thuộc phần tiếng Anh, giữ nguyên. |
| V04 | Dấu phẩy trước "và"              | Không có dấu phẩy: "A, B và C"               | "A, B, và C"; "…, và …"                                                                                     | Áp dụng cho cả liệt kê lẫn nối hai mệnh đề.                                                                                                                                                 |

### Ghi chú cách viết thay thế gạch dài (V01)

- Ngăn cách ý trong câu: dùng dấu phẩy, dấu hai chấm, ngoặc đơn, hoặc tách thành hai câu. Không thay bằng `-` có khoảng trắng hai bên chỉ để giữ nhịp cũ.
- Khoảng số hoặc ngày: "từ 2020 đến 2025", hoặc `2020-2025` (gạch ngắn, không khoảng trắng).
- Số âm hoặc phép trừ: dùng `-` (U+002D), không dùng `−`.
- Tên ghép, dấu nối từ: `-` như thường lệ.

## Văn bản hành chính và hồ sơ dự án: Nghị định 30/2020/NĐ-CP

Hồ sơ dự án, công văn, tờ trình, quyết định, biên bản, thuyết minh và các văn bản hành chính khác theo **Nghị định 30/2020/NĐ-CP** (Điều 7 đến 9, Phụ lục I, II, III). Chuẩn của Nhà nước thắng mục Quy định chung khi mâu thuẫn; chỗ nghị định không quy định thì dùng mục Quy định chung.

**Bắt buộc đọc `references/nghi-dinh-30.md` trước khi soạn loại văn bản này.** File đó chứa bảng tra nhanh theo loại, khổ giấy, lề, phông, cỡ chữ, các ô thể thức, số ký hiệu, địa danh, bố cục nội dung, chữ ký, nơi nhận, phụ lục, chữ viết tắt tên loại, mẫu trình bày, bản sao, viết hoa và cách giao văn bản. Không soạn từ trí nhớ.

Không cần đọc file đó với văn bản không thuộc nhóm hành chính (thư, báo cáo nội bộ, nội dung website, bài học thuật).

## Văn bản học thuật: APA 7

Mọi thứ tuân thủ **APA 7**: trích dẫn trong bài, danh mục tài liệu tham khảo, dấu câu, định dạng, cách viết số, bảng và hình. APA 7 thắng mục Quy định chung hoàn toàn, kể cả khi dùng en dash hay em dash theo APA. Đã đối chiếu với trang chính thức apastyle.apa.org:

- Khoảng trang: en dash `–`, không ghi "pp." (ví dụ `45–67`).
- Trích dưới 40 từ: đưa vào câu, đặt trong nháy kép. Từ 40 từ trở lên: tách thành khối riêng, không dùng nháy.
- Dấu phẩy và dấu chấm đặt trước nháy đóng, các dấu khác (hai chấm, chấm phẩy, dấu ba chấm) đặt sau nháy đóng.

Điểm khác không nêu ở đây: theo APA 7, không theo trí nhớ. Chưa chắc thì nói rõ chưa chắc.

## Cách rà trước khi giao

Skill chỉ có văn bản, nên rà bằng cách tự đọc lại bản nháp, không dùng script:

1. Xác định chuẩn áp dụng (bảng "Chọn chuẩn theo loại văn bản").
2. Rà từng dòng của bảng trong mục Quy định chung (hoặc quy tắc của chuẩn đã chọn): tìm trong phần tiếng Việt các dạng ở cột "Không dùng" và sửa theo cột "Dùng". Với APA 7 và Nghị định 30, theo quy định riêng của chuẩn đó.
3. Bỏ qua phần tiếng Anh và phần trích nguyên văn.
4. Khi giao file hoặc văn bản dài, nói ngắn gọn chuẩn đã áp dụng và đã đổi loại ký tự nào. Nói rõ đây là rà bằng cách đọc, chưa phải kiểm bằng công cụ.

## Điểm cần lưu ý

- Trong văn bản học thuật, APA 7 thắng quy tắc "và" và dấu phẩy trước "và" trong mục Quy định chung: trích dẫn trong ngoặc và danh mục tài liệu tham khảo dùng `&` khi APA yêu cầu; câu văn xuôi tiếng Việt vẫn dùng chữ "và". Nếu người dùng muốn dùng "và" cả trong trích dẫn, ghi lại tại đây.
- Cách áp APA 7 cho tài liệu và tác giả tiếng Việt (thứ tự tên, dịch tiêu đề, viết "và" thay vì "&"). Khi gặp, theo hướng dẫn chính thức của APA, hoặc quy định riêng của trường, tạp chí nơi nộp bài nếu có.
- Nháy đơn cong `‘…’` chỉ dùng khi trích lồng bên trong một trích dẫn đã dùng nháy kép (mục Quy định chung).
- Apostrophe trong từ tiếng Anh nằm giữa văn bản tiếng Việt (client's, don't) giữ nguyên.

## Cách cập nhật skill này

Khi gặp lỗi mới:

1. Quy tắc chung (ký tự, dấu câu, cách viết): thêm **một dòng ở cuối bảng trong mục Quy định chung** (mã V tiếp theo, ghi: quy tắc, dùng, không dùng, lý do). Không cần sửa chỗ nào khác. Quy tắc riêng của Nghị định 30 thì thêm vào mục H tương ứng trong `references/nghi-dinh-30.md` (mã H tiếp theo); quy tắc riêng của APA 7 thì thêm vào mục Văn bản học thuật.
2. Đóng gói lại thành file `.zip` (thư mục `viet-style/` làm gốc, bên trong có `SKILL.md` và `references/`) rồi tải lên lại.
