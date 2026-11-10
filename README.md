# Quỹ Vườn Mít - FC MisThy Website 🌟

Trang web gây quỹ FC MisThy (Vườn Mít) được tối ưu hoá lại thành dạng web tĩnh siêu nhẹ, mượt mà, giữ nguyên 100% hiệu ứng giao diện (Cosmic Glow, Glassmorphism, animations) và đã được bổ sung thêm khung **"QUÀ SINH NHẬT"** theo đúng yêu cầu.

---

## 🚀 1. Cách đưa lên GitHub & Tạo link Web trực tiếp (GitHub Pages)

### Bước 1: Tạo Repository mới trên GitHub
1. Truy cập: [https://github.com/new](https://github.com/new)
2. Đặt tên repository: **`vuon-mit-website`** (hoặc tên tùy thích).
3. Chọn chế độ: **Public** (để dùng được GitHub Pages miễn phí).
4. Nhấn **Create repository**.

### Bước 2: Đẩy toàn bộ code lên GitHub
Mở Terminal / PowerShell tại thư mục `C:\vuon-mit-website` và chạy các lệnh:
```bash
git add .
git commit -m "feat: clone website và thêm khung Quà Sinh Nhật"
git branch -M main
git remote add origin https://github.com/artrenn-sudo/vuon-mit-website.git
git push -u origin main
```
*(Nếu đã có sẵn remote origin, bạn chỉ cần chạy `git push -u origin main`)*

### Bước 3: Bật link Web chạy trực tiếp (GitHub Pages)
1. Vào repository vừa tạo trên GitHub: `https://github.com/artrenn-sudo/vuon-mit-website`
2. Chọn tab **Settings** -> Mục **Pages** (ở cột bên trái).
3. Tại phần **Build and deployment** -> **Source**: Chọn **Deploy from a branch**.
4. Dưới mục **Branch**: Chọn nhánh **`main`** và thư mục **`/(root)`** -> Nhấn **Save**.
5. Đợi 1-2 phút, GitHub sẽ cấp cho bạn một đường link chạy trực tiếp dạng:
   👉 **`https://artrenn-sudo.github.io/vuon-mit-website/`**

---

## ✏️ 2. Cách cập nhật số tiền "Quà Sinh Nhật" (Chỉ mất 10 giây)

Bạn không cần biết lập trình phức tạp và không cần chờ đợi deploy lâu:
1. Mở file [`index.html`](index.html).
2. Tìm đến dòng có chữ `QUÀ SINH NHẬT` (khoảng dòng 165).
3. Đổi số tiền trong thẻ `<p>`:
```html
<!-- SỬA SỐ TIỀN DƯỚI ĐÂY -->
<p id="qua-sinh-nhat-amount" class="font-bold text-white mb-2 mt-4 text-center" style="font-family: Goldman; font-size: clamp(1.5rem, 4vw, 2.5rem);">
  0 VND  <--- Đổi số tiền này (Ví dụ: 15,000,000 VND)
</p>
```
4. Lưu file và đẩy lên GitHub (`git add index.html && git commit -m "update qua sinh nhat" && git push`), trang web sẽ tự cập nhật ngay lập tức!

---

## 📂 3. Cấu trúc thư mục
- `index.html`: File HTML chính của trang web (đã tích hợp đầy đủ styling, animation, các khung dự án và khung Quà sinh nhật mới).
- `assets/`: Chứa ảnh mã QR ngân hàng (`QRcode.svg`) và stylesheet giao diện (`style.css`).
- `Vuon Mit-FC MisThy.html` & `Vuon Mit-FC MisThy_files/`: Bản sao gốc dự phòng khi cần đối chiếu.

