# 🎮 EduPlay – Học Vui Mỗi Ngày

Website học tập game hóa dành cho học sinh – bao gồm Toán, Tiếng Anh, Ngữ Văn.

## ✨ Tính năng

| Tính năng | Mô tả |
|---|---|
| 📚 Lý thuyết | Bài học với công thức, ví dụ minh họa |
| 🧩 Quiz | Trắc nghiệm tính điểm, phản hồi ngay lập tức |
| 🃏 Flashcard | Lật thẻ ôn từ vựng / khái niệm |
| 🏆 Bảng xếp hạng | So sánh điểm XP với bạn bè |
| ⭐ Hệ thống XP | Kiếm điểm kinh nghiệm sau mỗi bài quiz |
| 🔥 Streak | Theo dõi số ngày học liên tiếp |

## 🚀 Deploy lên GitHub Pages (Miễn phí)

### Bước 1 – Tạo Repository
1. Vào [github.com](https://github.com) → Đăng nhập
2. Nhấn **New repository**
3. Đặt tên: `hoc-vui` (hoặc tên bất kỳ)
4. Chọn **Public** → Nhấn **Create repository**

### Bước 2 – Upload file
1. Nhấn **Add file** → **Upload files**
2. Kéo thả file `index.html` vào
3. Nhấn **Commit changes**

### Bước 3 – Bật GitHub Pages
1. Vào **Settings** → **Pages** (menu bên trái)
2. Mục **Source**: chọn `Deploy from a branch`
3. Branch: chọn `main` → Folder: `/ (root)`
4. Nhấn **Save**
5. Chờ ~1 phút → URL của bạn sẽ là:
   ```
   https://<username>.github.io/<repo-name>/
   ```

## 📁 Cấu trúc file

```
/
└── index.html   ← Toàn bộ website trong 1 file
└── README.md    ← Hướng dẫn này
```

## ✏️ Cách thêm bài học / câu hỏi

Mở `index.html`, tìm phần `const subjects = { ... }` và chỉnh sửa:

### Thêm bài học lý thuyết
```js
lessons: [
  {
    title: 'Tên bài học',
    desc: 'Mô tả ngắn',
    content: `<h3>Tiêu đề</h3><p>Nội dung HTML...</p>`
  }
]
```

### Thêm câu hỏi Quiz
```js
quiz: [
  {
    q: 'Câu hỏi của bạn?',
    opts: ['Đáp án A', 'Đáp án B', 'Đáp án C', 'Đáp án D'],
    ans: 1  // Index của đáp án đúng (0=A, 1=B, 2=C, 3=D)
  }
]
```

### Thêm Flashcard
```js
flashcards: [
  {
    front: 'Mặt trước thẻ',
    phonetic: 'Phiên âm / chú thích',
    back: 'Định nghĩa / giải thích',
    hint: 'Gợi ý, ví dụ'
  }
]
```

## 🎨 Thay đổi màu sắc

Tìm `:root { ... }` trong CSS để thay đổi màu chủ đạo:
```css
--accent1: #ff6b6b;   /* Đỏ */
--accent2: #ffd93d;   /* Vàng */
--accent3: #6bcb77;   /* Xanh lá */
--accent4: #4d96ff;   /* Xanh dương */
--accent5: #c77dff;   /* Tím */
```

## 📱 Tương thích
- ✅ Desktop, Laptop
- ✅ Điện thoại, Tablet
- ✅ Không cần cài thêm gì – chỉ 1 file HTML

---
Made with ❤️ for Vietnamese students
