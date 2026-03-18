# CLAUDE.md — Paul's Medical Workspace
> Last updated: 2026-03-18 (rev 3)
> Machine: LT-E7470 | User: JamesBond

---

## 👤 About Me

- **Tên:** Paul
- **Năm:** Y4 — Đại học Nguyễn Tất Thành
- **Rotation hiện tại:** Nội khoa — Bệnh Viện Nhân Dân Gia Định
- **Mục tiêu:** Bác sĩ Nội Trú đại học Y Dược thành phố Hồ Chí Minh
- **Side business:** Quán Bòn Bòn (nhà hàng Việt Nam)
- **Đầu tư:** Chứng khoán (VND, HPG, POM — HOSE/HNX)

---

## 🌐 Language Rules

- **Respond in:** Mix Vietnamese + English
  - Vietnamese → medical content, bệnh án, Anki cards, Obsidian notes
  - English → code, file paths, technical commands
- **Medical terms:** Always use Vietnamese clinical terminology
  - Examples: biện luận, HCTH, VCTC, CLS, bệnh án, chẩn đoán, điều trị

---

## ⚡ Behavior Rules

- **Big tasks** (creating PPTX, bulk Anki, restructuring files): **ASK FIRST**, describe plan, wait for confirmation
- **Small tasks** (single Anki card, quick note, rename file): Do immediately
- **Errors:** Tell me clearly what went wrong in Vietnamese
- **Done:** Always confirm when complete with a short summary

### What counts as a "big task":
- Creating or editing PPTX files
- Generating more than 5 Anki cards at once
- Moving or renaming multiple files
- Pushing anything to Anki (always STAGING first)
- Posting to Notion or social media
- Deleting any file

---

## 📁 File Paths

```
Obsidian Vault:         C:\Paul Obsidian Vault\
Instructions folder:    C:\Paul Obsidian Vault\Cowork_Instructions\
Daily Logs:             C:\Paul Obsidian Vault\00_Daily_Logs\
Cases:                  C:\Paul Obsidian Vault\01_Cases\
Exam Preps:             C:\Paul Obsidian Vault\02_Exam_Preps\
Presentations:          C:\Paul Obsidian Vault\03_Presentations\
Templates:              C:\Paul Obsidian Vault\TEMPLATES\
Medical content:        C:\Paul Obsidian Vault\Môn chuyên ngành\
Desktop:                C:\Users\JamesBond\Desktop\
Downloads:              C:\Users\JamesBond\Downloads\
Google Drive:           C:\Users\JamesBond\Google Drive\My Drive\
Bệnh án output:         G:\My Drive\BỆNH ÁN VTT\
```

---

## 🃏 Anki Rules

> ⚠️ ĐỌC KỸ — Sai format là plugin không nhận!
> Full rules: `C:\Paul Obsidian Vault\Cowork_Instructions\_Anki_Instructions.md`

### Triết lý cốt lõi

> "Hiểu trước, nhớ sau. Mỗi card = 1 sự thật. Basic buộc suy luận — Cloze chỉ điền vào chỗ trống."

**Ưu tiên loại card:**
- 🥇 **Basic (`#flashcard`) là mặc định** — ≥ 70% mỗi batch
- 🥈 **Cloze (`#clozecard`) chỉ dùng cho con số / ngưỡng / liều** — ≤ 30% mỗi batch
- **Nếu phân vân → chọn Basic**

### Nguyên tắc Self-Contained
> Mỗi thẻ phải tự đứng được khi đọc random lúc 6h sáng, không cần nhớ context từ session học.

Checklist trước khi tạo card:
- [ ] Tên bệnh / thuốc / hệ thống có trong câu hỏi không?
- [ ] Không có đại từ mơ hồ (nó, thuốc này, tiêu chí này)?
- [ ] Viết tắt lần đầu có chú thích không?
- [ ] Chỉ có 1 đáp án đúng không?

### Workflow (KHÔNG bỏ bước nào)

**B1 — Nhận source:** Text paste / PDF / ảnh slide / link web — đọc hiểu cấu trúc trước

**B2 — Xác nhận tên bệnh:** KHÔNG tự đoán, hỏi Paul trước

**B3 — Xác định file đích:**
- Tên file = tên bệnh VIẾT HOA: `SUY TIM.md`, `COPD.md`
- Path: `C:\Paul Obsidian Vault\Môn chuyên ngành\[Chuyên khoa]\[TÊN BỆNH].md`
- Tìm file cũ trước — KHÔNG tạo `TĂNG HUYẾT ÁP 1.md`

**B4 — Dò trùng trong vault:**
- Đọc toàn bộ file đích hiện có
- Phân loại: trùng y hệt → bỏ qua | card cũ kém hơn → tạo mới + ghi chú đề xuất thay thế | góc hỏi khác → tạo thêm
- KHÔNG tự xóa card cũ — chỉ báo cáo để Paul quyết định

**B5 — Tra Deck Name** (xem bảng bên dưới)

**B6 — Preview 5 cards → chờ duyệt:**
```
📋 Preview 5 cards:
1. - [câu hỏi]? #flashcard 
   - [đáp án]
2. - [câu cloze {1:số}] #clozecard 
...
📊 ~[X] cards ([A] Basic + [B] Cloze)
🔍 Dò trùng: [Y] bỏ qua | [Z] đề xuất thay thế
📁 File: C:\Paul Obsidian Vault\...\[TÊN BỆNH].md
🗂️ Deck: [deck name]
Duyệt không Paul?
```

**B7 — Append sau khi duyệt:** Append vào cuối `# OBISIDIAN TO ANKI`, KHÔNG xóa cards cũ

### Cú pháp

**Basic Card (MẶC ĐỊNH):**
```
- [Câu hỏi rõ ràng, có tên bệnh/hệ thống]? #flashcard 
- Đáp án dòng 1
- Đáp án dòng 2
```

**Cloze Card (chỉ cho con số/ngưỡng/liều):**
```
- Câu hoàn chỉnh với {1:con số} được ẩn #clozecard 
```

⚠️ Dùng `{1:...}` — KHÔNG dùng `{{c1::...}}`
⚠️ Có khoảng trắng sau tag: `#flashcard ` và `#clozecard ` (space cuối)
⚠️ Giữ nguyên typo **"OBISIDIAN"** trong header file

### Deck Name Map

**Nội khoa:**

| Bệnh | Deck |
|---|---|
| SUY TIM | `2. NỘI KHOA::TIM MẠCH::SUY TIM` |
| TĂNG HUYẾT ÁP | `2. NỘI KHOA::TIM MẠCH::TĂNG HUYẾT ÁP` |
| HỘI CHỨNG VÀNH CẤP | `2. NỘI KHOA::TIM MẠCH::HỘI CHỨNG VÀNH CẤP` |
| HỘI CHỨNG VÀNH MẠN | `2. NỘI KHOA::TIM MẠCH::HỘI CHỨNG VÀNH MẠN` |
| RỐI LOẠN LIPID MÁU | `2. NỘI KHOA::TIM MẠCH::RỐI LOẠN LIPID MÁU` |
| Hẹp / Hở van tim | `2. NỘI KHOA::TIM MẠCH::BỆNH VAN TIM::[tên van]` |
| COPD | `2. NỘI KHOA::HÔ HẤP::COPD` |
| HEN | `2. NỘI KHOA::HÔ HẤP::HEN` |
| VIÊM PHỔI | `2. NỘI KHOA::HÔ HẤP::VIÊM PHỔI` |
| TRÀN DỊCH MÀNG PHỔI | `2. NỘI KHOA::HÔ HẤP::TRÀN DỊCH MÀNG PHỔI` |
| XƠ GAN | `2. NỘI KHOA::TIÊU HÓA::XƠ GAN` |
| VIÊM GAN | `2. NỘI KHOA::TIÊU HÓA::VIÊM GAN` |
| VIÊM TỤY CẤP | `2. NỘI KHOA::TIÊU HÓA::VIÊM TUY CẤP` |
| XUẤT HUYẾT TIÊU HÓA | `2. NỘI KHOA::TIÊU HÓA::XUẤT HUYẾT TIÊU HÓA` |
| VIÊM - LOÉT DẠ DÀY TÁ TRÀNG | `2. NỘI KHOA::TIÊU HÓA::VIÊM - LOÉT DẠ DÀY TÁ TRÀNG` |
| TRÀO NGƯỢC DẠ DÀY THỰC QUẢN | `2. NỘI KHOA::TIÊU HÓA::TRÀO NGƯỢC DẠ DÀY THỰC QUẢN` |
| HỘI CHỨNG THẬN HƯ | `2. NỘI KHOA::THẬN::HỘI CHỨNG THẬN HƯ` |
| BỆNH THẬN MẠN | `2. NỘI KHOA::THẬN::BỆNH THẬN MẠN` |
| TỔN THƯƠNG THẬN CẤP | `2. NỘI KHOA::THẬN::TỔN THƯƠNG THẬN CẤP` |
| ĐÁI THÁO ĐƯỜNG | `2. NỘI KHOA::THẬN::ĐÁI THÁO ĐƯỜNG` |
| HỘI CHỨNG CUSHING | `2. NỘI KHOA::THẬN::HỘI CHỨNG CUSHING` |

**Nhi khoa:** `5. Nhi khoa::NHI 1::[Tên bệnh]`

**Ngoại khoa (Đề cương YDS):**

| Tên chủ đề | Deck |
|---|---|
| SỰ LÀNH VẾT THƯƠNG | `Đề cương YDS::01. Sự lành vết thương` |
| NHIỄM TRÙNG NGOẠI KHOA | `Đề cương YDS::02. Nhiễm trùng Ngoại Khoa` |
| SỐC CHẤN THƯƠNG | `Đề cương YDS::03. Sốc chấn thương` |
| ĐAU LIÊN QUAN PHẪU THUẬT | `Đề cương YDS::04. Đau liên quan với phẫu thuật` |
| NGOẠI KHOA VÀ BỆNH MẠN TÍNH | `Đề cương YDS::05. Ngoại khoa và các bệnh mạn tính` |
| RỐI LOẠN ĐÔNG MÁU / TRUYỀN MÁU | `Đề cương YDS::06. Rối loạn đông máu - cầm máu và truyền máu` |
| VIÊM RUỘT THỪA | `Đề cương YDS::07. Viêm ruột thừa` |
| VIÊM PHÚC MẠC | `Đề cương YDS::08. Viêm phúc mạc` |
| CHẤN THƯƠNG BỤNG | `Đề cương YDS::09. Chấn thương bụng - vết thương bụng` |
| LOÉT DẠ DÀY TÁ TRÀNG (NGOẠI) | `Đề cương YDS::10. Loét dạ dày tá tràng` |
| TẮC RUỘT CƠ HỌC | `Đề cương YDS::11. Tắc ruột cơ học` |
| CO THẮT TÂM VỊ | `Đề cương YDS::12. Co thắt tâm vị` |
| UNG THƯ THỰC QUẢN | `Đề cương YDS::13. Ung thư thực quản` |
| UNG THƯ DẠ DÀY | `Đề cương YDS::14. Ung thư dạ dày` |
| UNG THƯ ĐẠI TRỰC TRÀNG | `Đề cương YDS::15. Ung thư đại trực tràng` |
| SỎI ĐƯỜNG MẬT / SỎI TÚI MẬT | `Đề cương YDS::16. Sỏi đường mật và sỏi túi mật` |
| UNG THƯ GAN NGUYÊN PHÁT | `Đề cương YDS::17. Ung thư gan nguyên phát` |
| UNG THƯ TỤY | `Đề cương YDS::18. Ung thư tụy` |
| THOÁT VỊ | `Đề cương YDS::19. Thoát vị` |
| TRĨ - NHIỄM TRÙNG HẬU MÔN | `Đề cương YDS::20. Trĩ - Nhiễm trùng hậu môn` |

**Sản phụ khoa (Chủ đề BSNT):**

| Tên chủ đề | Deck |
|---|---|
| XUẤT HUYẾT TỬ CUNG BẤT THƯỜNG | `4. Sản phụ khoa::Chủ đề BSNT::01. Xuất huyết tử cung bất thường` |
| VIÊM VÙNG CHẬU CẤP | `4. Sản phụ khoa::Chủ đề BSNT::02. Viêm vùng chậu cấp` |
| TIẾT DỊCH ÂM ĐẠO BẤT THƯỜNG | `4. Sản phụ khoa::Chủ đề BSNT::03. Tiết dịch âm đạo bất thường` |
| KHỐI U VÙNG CHẬU | `4. Sản phụ khoa::Chủ đề BSNT::04. Khối u vùng chậu` |
| TẦM SOÁT UNG THƯ CỔ TỬ CUNG | `4. Sản phụ khoa::Chủ đề BSNT::05. Tầm soát ung thư cổ tử cung` |
| ĐAU VÚ | `4. Sản phụ khoa::Chủ đề BSNT::06. Đau vú` |
| KHỐI U VÚ | `4. Sản phụ khoa::Chủ đề BSNT::07. Khối u vú` |
| TRÁNH THAI / TRÁNH THAI KHẨN CẤP | `4. Sản phụ khoa::Chủ đề BSNT::08. Tránh thai` |
| PHÁ THAI | `4. Sản phụ khoa::Chủ đề BSNT::09. Phá thai` |
| VẤN ĐỀ NỬA ĐẦU THAI KỲ | `4. Sản phụ khoa::Chủ đề BSNT::10. Các vấn đề thường gặp nửa đầu thai kỳ` |
| XUẤT HUYẾT ÂM ĐẠO 3 THÁNG ĐẦU | `4. Sản phụ khoa::Chủ đề BSNT::11. Xuất huyết âm đạo 3 tháng đầu thai kỳ` |
| SUY THAI | `4. Sản phụ khoa::Chủ đề BSNT::12. Suy thai` |
| THAI GIỚI HẠN TĂNG TRƯỞNG | `4. Sản phụ khoa::Chủ đề BSNT::13. Thai giới hạn tăng trưởng trong tử cung` |
| SINH NON | `4. Sản phụ khoa::Chủ đề BSNT::14. Sinh non` |
| VẾT MỔ CŨ LẤY THAI | `4. Sản phụ khoa::Chủ đề BSNT::15. Vết mổ cũ lấy thai` |
| TĂNG HUYẾT ÁP THAI KỲ | `4. Sản phụ khoa::Chủ đề BSNT::16. Tăng huyết áp thai kỳ` |
| ĐÁI THÁO ĐƯỜNG THAI KỲ | `4. Sản phụ khoa::Chủ đề BSNT::17. Đái tháo đường thai kỳ` |
| CHĂM SÓC TRONG CHUYỂN DẠ | `4. Sản phụ khoa::Chủ đề BSNT::18. Chăm sóc cơ bản trong chuyển dạ` |
| CẤP CỨU SẢN KHOA | `4. Sản phụ khoa::Chủ đề BSNT::19. Cấp cứu sản khoa` |
| CHĂM SÓC HẬU SẢN | `4. Sản phụ khoa::Chủ đề BSNT::20. Chăm sóc hậu sản` |
| CHO CON BÚ SỮA MẸ | `4. Sản phụ khoa::Chủ đề BSNT::21. Cho con bú sữa mẹ` |
| VÔ KINH - RỐI LOẠN PHÓNG NOÃN | `4. Sản phụ khoa::Chủ đề BSNT::22. Vô kinh - rối loạn phóng noãn` |

> ⚠️ Tên không có trong bảng trên → **hỏi Paul deck name trước khi tạo**

### Vault Structure
```
Môn chuyên ngành\
├── Nội\
│   ├── 1. TIM MẠCH\
│   ├── 2. HÔ HẤP\
│   ├── 3. TIÊU HÓA\
│   └── 4. THẬN - TIẾT NIỆU\
├── Nhi\
│   ├── HÔ HẤP\ | THẬN\ | TIM MẠCH\ | TIÊU HÓA\ | NHIỄM\ | HUYẾT HỌC\ | CẤP CỨU\
├── Ngoại\
└── Sản\
```

### KHÔNG làm (vi phạm nghiêm trọng)
- Dùng `{{c1::...}}` thay vì `{1:...}`
- Tạo file trùng tên trong vault
- Dùng deck Ngoại/Sản chưa xác nhận
- Push thẳng vào Anki — workflow: Obsidian → plugin → Anki
- Tạo Cloze cho nội dung không phải con số/ngưỡng/liều

---

## 📄 Bệnh Án Nội Khoa Rules

### Template
- **Google Doc template (nguồn chính thức):**
  `https://docs.google.com/document/d/1zLcWUUoWKKEu4jPRAE7_C7CIJgFdQZ7g3hz2WjLGcpI/edit`
- Fetch nội dung từ link này trước khi điền bệnh án
- Đây vừa là template tham khảo vừa là file mẫu gốc
- Full rules: `C:\Paul Obsidian Vault\Cowork_Instructions\_BenhAn_Instructions.md`

### Input từ Paul
> ⚠️ **Paul gửi TEXT** (không gửi ảnh) để tiết kiệm token xử lý.
> Paul sẽ paste trực tiếp nội dung sổ lâm sàng dạng text vào chat.

### Workflow

**B1 — Nhận text từ Paul:**
- Paul paste text ghi chép lâm sàng từ sổ tay
- Đọc toàn bộ, xác định các thông tin có / còn thiếu

**B2 — Fetch template:**
- Fetch Google Doc: `1zLcWUUoWKKEu4jPRAE7_C7CIJgFdQZ7g3hz2WjLGcpI`
- Đọc cấu trúc 12 phần và các trường `@@` cần điền

**B3 — Điền vào mẫu:**
- Thay thế tất cả `@@` bằng số liệu thực tế
- Phần KHÁM: mặc định BÌNH THƯỜNG — nếu text Paul ghi bất thường → sửa đúng mục

**B4 — Preview trước khi lưu:**
```
✅ Đã điền: [list các mục đã có đủ data]
⚠️ Khám bất thường đã thêm: [list từng mục]
❓ Còn thiếu: [list các trường không có data]
CHỜ xác nhận Paul trước khi lưu.
```

**B5 — Lưu file sau khi Paul xác nhận:**
- Save to: `G:\My Drive\BỆNH ÁN VTT\BA_[TenBenh]_[NgayTao].docx`

### Cấu trúc 12 phần

```
1.  PHẦN HÀNH CHÍNH (họ tên, giới, ngày sinh, dân tộc, địa chỉ, nghề nghiệp,
    ngày giờ nhập viện, ngày giờ làm bệnh án, khoa, phòng-giường)
2.  LÝ DO NHẬP VIỆN
3.  BỆNH SỬ
    1. Trước lúc nhập viện
    2. Tình trạng lúc nhập viện
    3. Diễn tiến bệnh phòng
    4. Tình trạng hiện tại
4.  TIỀN SỬ
    1. Bản thân: Nội khoa / Ngoại khoa / Dị ứng / Thói quen / Dịch tễ
    2. Gia đình
5.  LƯỢC QUA CÁC CƠ QUAN
    (Toàn thân / Đầu mặt cổ / Hô hấp / Tim mạch / Tiêu hóa /
    Tiết niệu / Thần kinh / Cơ xương khớp — mặc định "không...")
6.  KHÁM (mặc định BÌNH THƯỜNG — xem bảng bên dưới)
7.  TÓM TẮT BỆNH ÁN
8.  ĐẶT VẤN ĐỀ
9.  CHẨN ĐOÁN (sơ bộ + phân biệt)
10. ĐỀ NGHỊ CẬN LÂM SÀNG
11. KẾT QUẢ CẬN LÂM SÀNG
12. HƯỚNG ĐIỀU TRỊ (cấp cứu / nguyên nhân / triệu chứng-biến chứng / bệnh đi kèm)
```

### Các trường @@ trong phần KHÁM

| Vị trí | Trường | Ví dụ |
|---|---|---|
| Tổng trạng | Mạch: @@@ lần/phút | 96 |
| Tổng trạng | Huyết áp: @@/xx mmHg | 130/80 |
| Tổng trạng | Nhiệt độ: @@ độ C | 37.2 |
| Tổng trạng | Nhịp thở: @@ lần/phút | 18 |
| Tổng trạng | SpO2: @@% / khí trời | 98 |
| Tổng trạng | Cân nặng: @@ kg | 65 |
| Tổng trạng | Chiều cao: @@ cm | 165 |
| Tổng trạng | BMI: @@ kg/m² | 23.9 |
| Tim mạch | Diện đập mỏm tim @@ cm² | 2 |
| Tim mạch | Nhịp tim: @@ lần/phút | 96 |
| Bụng | Nhu động ruột @@ lần/phút | 4 |

### Khám bất thường — Cách xử lý

| Mặc định trong mẫu | Nếu bất thường → sửa thành |
|---|---|
| Không phù | Phù 2 chi dưới / Phù mặt |
| Không ran phổi | Ran ẩm 2 đáy phổi / Ran nổ |
| Rì rào phế nang êm dịu | Rì rào phế nang giảm bên (T)/(P) |
| Không ghi nhận âm thổi | Âm thổi tâm thu 2/6 ở [vị trí] |
| Tĩnh mạch cổ không nổi | Tĩnh mạch cổ nổi ở tư thế 45° |
| Gan, lách không sờ | Gan to @@ cm dưới bờ sườn (P) |
| Không vàng da | Vàng da, vàng mắt |
| Cổ mềm | Cổ cứng, Kernig (+), Brudzinski (+) |
| Sức cơ 5/5 | Sức cơ chi [trên/dưới] [P/T] [x]/5 |

---

## 🖥️ PPTX Bệnh Án Rules

### Template
- Hospital: Bệnh Viện Nhân Dân Gia Định (Nội khoa)
- Template: `C:\Users\JamesBond\Desktop\Templates\benh-an-noi-khoa.pptx`
- If not found → ask Paul before proceeding

### Slide Structure
```
Slide 1:  Tiêu đề — Tên BN, Tuổi, Giới, Ngày vào viện
Slide 2:  Lý do vào viện
Slide 3:  Bệnh sử
Slide 4:  Tiền sử (bản thân + gia đình)
Slide 5:  Khám lâm sàng
Slide 6:  Cận lâm sàng
Slide 7:  Chẩn đoán sơ bộ + Biện luận
Slide 8:  Chẩn đoán xác định
Slide 9:  Điều trị
Slide 10: Tiên lượng + Dự phòng
```

### Output
- Save to: `G:\My Drive\BỆNH ÁN VTT\[TenBenh]_[NgayTao].pptx`
- Always confirm filename with Paul before saving

---

## 📓 Obsidian Notes Rules

### Note Template
```markdown
# [Tên Bệnh]

**Chuyên khoa:** [Specialty]
**Tags:** #[specialty] #[disease]
**Ngày tạo:** [Date]

## Định nghĩa
## Nguyên nhân
## Triệu chứng lâm sàng
## Cận lâm sàng
## Chẩn đoán
## Điều trị
## Tiên lượng
## Nguồn tham khảo

# OBISIDIAN TO ANKI
TARGET DECK: [deck name]
```

---

## ✅ Notion Rules

> Full rules: `C:\Paul Obsidian Vault\Cowork_Instructions\_Notion_Instructions.md`

### Hệ thống: Paul's PARA (Ultimate Brain template)

**Trang chủ:** `c5463c4e-cad0-4586-9e8a-750cfcf7f3a9`

**Database Collection IDs:**

| Database | Collection ID |
|---|---|
| All Tasks [UB] | `12db13dc-70d3-47c3-9128-e3e4c197fc18` |
| Projects [UB] | `6757de3d-a871-46d7-81a8-c482a003ac71` |
| Areas & Resources [UB] | `8ce7c6a5-a27a-4cef-b2ad-88d63e72c209` |
| Goals [UB] | `0ce59c68-75ad-438e-8535-7390f0f2ab01` |
| Notes [UB] | `472f291a-894a-4221-ac4b-f448c558eb93` |

**Task Views:**

| View | Lọc |
|---|---|
| Task Inbox | Chưa có project/due |
| Today | Due = hôm nay |
| Tomorrow | Due = ngày mai |
| Next 7 Days | Due trong 7 ngày tới |
| Cold Tasks | Không có due date |
| Priority View | HIGH priority |

### Task Properties quan trọng

| Property | Giá trị hợp lệ |
|---|---|
| `Priority` | `🚨HIGH` / `🧀 Medium` / `🧊 Low` |
| `Done` | `__YES__` / `__NO__` |
| `Smart List` | `Do Next` / `Delegated` / `Someday` |
| `Kanban Status` | `To Do` / `Doing` / `Done` |
| `Contexts` | `High-Energy` / `Low-Energy` / `Errand` / `Home` / `Office` / `Social` |

### Project Properties quan trọng

| Property | Giá trị hợp lệ |
|---|---|
| `Status` | `To Do` / `Doing` / `Done` / `On Hold` / `Ongoing` |
| `Priority` | `__YES__` (checkbox) |

### Workflows

**Capture nhanh:** Tạo task → title + Priority (default Medium) + Due nếu có. KHÔNG hỏi thêm khi capture.

**Khi nào tạo Project (không phải Task):** Có > 2 tasks liên quan + outcome rõ ràng

**Update nhanh:**
- "Done rồi" → `Done = true` / `Status = Done + Completed = today`
- "Hoãn sang [ngày]" → `Snooze date` (GIỮ NGUYÊN Due date)
- "On hold" → `Status = On Hold + Review Notes = lý do`

**Task naming:** Bắt đầu bằng động từ: Đọc / Viết / Gọi / Hoàn thành / Ôn / Tạo

**Priority guidelines:**
- `🚨HIGH` → Deadline hôm nay/ngày mai, thi BSNT, Quán Bòn Bòn khẩn
- `🧀 Medium` → Deadline trong tuần
- `🧊 Low` → Someday, cold tasks

### Areas của Paul
Y học/BSNT | Quán Bòn Bòn | Tài chính/Đầu tư | Sức khoẻ | Học tập liên tục | Gia đình | Tech/AI

### Safety Rules Notion
- KHÔNG xóa — chỉ Archive hoặc Done
- KHÔNG tự suy đoán Area/Goal → hỏi Paul
- KHÔNG đặt Due date khi Paul không đề cập
- LUÔN báo cáo sau mỗi thao tác

---

## 🏥 Current Rotation Context

**Bệnh Viện Nhân Dân Gia Định — Nội Khoa**

Focus cases (tên theo deck Anki):
- **Tim mạch:** SUY TIM, TĂNG HUYẾT ÁP, HỘI CHỨNG VÀNH CẤP, HỘI CHỨNG VÀNH MẠN, BỆNH VAN TIM, RỐI LOẠN LIPID MÁU
- **Hô hấp:** COPD, VIÊM PHỔI, HEN, TRÀN DỊCH MÀNG PHỔI
- **Thận:** TỔN THƯƠNG THẬN CẤP, BỆNH THẬN MẠN, HỘI CHỨNG THẬN HƯ, ĐÁI THÁO ĐƯỜNG
- **Tiêu hóa:** XƠ GAN, XUẤT HUYẾT TIÊU HÓA, VIÊM GAN, VIÊM TỤY CẤP, VIÊM-LOÉT DẠ DÀY TÁ TRÀNG, TRÀO NGƯỢC DẠ DÀY THỰC QUẢN

---

## 📱 iPhone Remote Control

When Paul sends tasks from iPhone:
- He is at the hospital, cannot check immediately
- Complete fully, save to correct folder
- Send a short completion summary he can read quickly
- If blocked → describe issue clearly and wait, do NOT guess

---

## 🚫 Never Do Without Asking

- Delete any file
- Push cards directly to Anki (always STAGING first)
- Post on social media
- Send emails or messages
- Modify template files
- Access personal/financial data
