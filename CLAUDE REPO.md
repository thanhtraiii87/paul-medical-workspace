# CLAUDE.md — Paul's Medical Workspace
> Last updated: 2026-03-11
> Machine: LT-E7470 | User: JamesBond

---

## 👤 About Me

- **Tên:** Paul
- **Năm:** Y4 — Đại học Nguyễn Tất Thành
- **Rotation hiện tại:** Nội khoa — Bệnh Viện Nhân Dân Gia Định
- **Mục tiêu:** BSNT UMP HCMC → Sở hữu bệnh viện tư nhân
- **Side business:** Quán Bòn Bòn (nhà hàng Việt Nam)
- **Đầu tư:** Chứng khoán

---

## 🌐 Language Rules

- **Respond in:** Mix Vietnamese + English
  - Vietnamese → for medical content, bệnh án, Anki cards, Obsidian notes
  - English → for code, file paths, technical commands
- **Medical terms:** Always use Vietnamese clinical terminology
  - Examples: biện luận, HCTH, VCTC, CLS, bệnh án, chẩn đoán, điều trị

---

## ⚡ Behavior Rules

- **Big tasks** (creating PPTX, bulk Anki, restructuring files): **ASK ME FIRST**, describe what you'll do, wait for my confirmation
- **Small tasks** (single Anki card, quick note, rename file): Do it immediately, no questions
- **Errors:** Tell me clearly what went wrong in Vietnamese
- **Done:** Always confirm when task is complete with a short summary

### What counts as a "big task":
- Creating or editing PPTX files
- Generating more than 5 Anki cards at once
- Moving or renaming multiple files
- Pushing anything to Anki (always use STAGING first)
- Posting to Notion or social media
- Deleting any file

---

## 📁 File Paths

```
Obsidian Vault:     C:/Obsidian/Medical/
Anki STAGING:       C:/Obsidian/Medical/STAGING/
Desktop:            C:/Users/JamesBond/Desktop/
Downloads:          C:/Users/JamesBond/Downloads/
Cases folder:       C:/Users/JamesBond/Desktop/Cases/
Templates folder:   C:/Users/JamesBond/Desktop/Templates/
```

---

## 🃏 Anki Rules

### Deck Naming Convention
```
1. Giải phẫu
2. Sinh lý
3. Dược lý
4. Nội khoa::NOI 1::[Bệnh]
5. Nhi khoa::NHI 1::[Bệnh]
6. Ngoại khoa
7. Sản phụ khoa
```

### Card Format (Cloze)
```
{{c1::Câu trả lời}} là biểu hiện của {{c2::bệnh}}
```

### Tags (always add all 3 layers)
```
Layer 1 - Type:       #clozecard  OR  #flashcard
Layer 2 - Specialty:  #noi-khoa | #nhi-khoa | #ngoai-khoa | #san-khoa
Layer 3 - Category:   #chan-doan | #dieu-tri | #can-lam-sang | #tieu-chuan | #bien-luan
Disease tag:          #[ten-benh]  (vd: #HCTH #VCTC #suy-tim #COPD)
```

### Two-Step Staging Workflow
1. **Claude saves cards** → `C:/Obsidian/Medical/STAGING/[TenBenh].md`
2. **Paul reviews** on iPhone via Obsidian Mobile
3. **Paul approves** → Claude pushes to Anki deck via AnkiConnect
4. **NEVER push directly to Anki** without Paul's approval

### AnkiConnect
- Port: `8765`
- Anki must be open on PC for AnkiConnect to work
- Always verify connection before bulk operations

---

## 🖥️ PPTX Bệnh Án Rules

### Template
- Hospital: Bệnh Viện Nhân Dân Gia Định (Nội khoa)
- Use template file at: `C:/Users/JamesBond/Desktop/Templates/benh-an-noi-khoa.pptx`
- If template not found → ask Paul before proceeding

### Slide Structure (Bệnh Án Nội Khoa)
```
Slide 1:  Tiêu đề — Tên bệnh nhân, Tuổi, Giới, Ngày vào viện
Slide 2:  Lý do vào viện
Slide 3:  Bệnh sử
Slide 4:  Tiền sử (bản thân + gia đình)
Slide 5:  Khám lâm sàng
Slide 6:  Cận lâm sàng (CLS)
Slide 7:  Chẩn đoán sơ bộ + Biện luận
Slide 8:  Chẩn đoán xác định
Slide 9:  Điều trị
Slide 10: Tiên lượng + Dự phòng
```

### Output
- Save to: `C:/Users/JamesBond/Desktop/Cases/[TenBenh]_[NgayTao].pptx`
- Always confirm filename with Paul before saving

---

## 📓 Obsidian Notes Rules

### Vault Structure
```
C:/Obsidian/Medical/
├── Nội khoa/
│   ├── Tim mạch/
│   ├── Hô hấp/
│   ├── Thận - Tiết niệu/
│   ├── Nội tiết/
│   └── Tiêu hóa/
├── Nhi khoa/
├── Ngoại khoa/
├── Sản phụ khoa/
└── STAGING/
```

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
```

---

## ✅ Notion Rules

- **Workspace:** PARA system
- **Daily tasks:** Add to "Inbox" database
- **Medical cases:** Add to "Projects → Rotation Gia Định"
- **Quán Bòn Bòn:** Add to "Projects → Marketing Quán Bòn Bòn"
- Always confirm before creating or modifying Notion pages

---

## 🏥 Current Rotation Context

**Bệnh Viện Nhân Dân Gia Định — Nội Khoa**

Common cases to focus on:
- Tim mạch: Suy tim, Tăng huyết áp, NMCT
- Hô hấp: COPD, Viêm phổi, Hen phế quản
- Thận: Suy thận cấp/mạn
- Nội tiết: Đái tháo đường type 2, Rối loạn tuyến giáp
- Tiêu hóa: Xơ gan, Xuất huyết tiêu hóa trên

---

## 📱 iPhone Remote Control

When Paul sends tasks from iPhone, assume:
- He is at the hospital and cannot check immediately
- Complete the task fully and save results to correct folder
- Send a short completion summary he can read quickly
- If blocked, describe the issue clearly and wait — do NOT guess

---

## 🚫 Never Do Without Asking

- Delete any file
- Push cards directly to Anki (always STAGING first)
- Post on social media
- Send emails or messages
- Modify template files
- Access personal/financial data
