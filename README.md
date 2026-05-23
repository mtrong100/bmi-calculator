# BMI Calculator

Ứng dụng tính chỉ số khối cơ thể (BMI) hiện đại, hỗ trợ song ngữ Việt – Anh, chuẩn Material Design 3, đầy đủ tính năng PWA.

---

## Tính năng

- **Tính BMI** theo hệ mét (cm/kg) và hệ Anh (in/lb)
- **Song ngữ** Tiếng Việt / English — chuyển đổi tức thì
- **Ba chế độ giao diện**: Sáng · Tối · Theo hệ thống
- **Ghi nhớ tuỳ chỉnh** bằng localStorage (ngôn ngữ, theme, giới tính, đơn vị, số liệu đầu vào)
- **Biểu đồ gauge** trực quan cho vị trí BMI trên thang đo
- **Bảng phân loại** BMI 7 mức (WHO)
- **Khoảng cân nặng lý tưởng** dựa trên chiều cao
- **Accordion FAQ** về BMI
- **Responsive** — điện thoại, tablet, iPad, laptop, PC
- **PWA** — cài đặt như ứng dụng native, hỗ trợ offline
- **Favicon** phong cách One UI 8 (SVG + PNG đa kích thước)
- **Font** Be Vietnam Pro — hỗ trợ đầy đủ tiếng Việt

---

## Cấu trúc thư mục

```
bmi-calculator/
├── index.html          # Ứng dụng chính (HTML + CSS + JS)
├── manifest.json       # PWA Web App Manifest
├── sw.js               # Service Worker (cache offline)
├── favicon.svg         # Favicon SVG (One UI 8 style)
├── README.md           # Tài liệu này
└── icons/
    ├── icon-72.png
    ├── icon-96.png
    ├── icon-128.png
    ├── icon-144.png
    ├── icon-152.png
    ├── icon-192.png
    ├── icon-384.png
    └── icon-512.png
```

---

## Cách sử dụng

### Chạy trực tiếp
Mở file `index.html` trong trình duyệt. Để PWA & Service Worker hoạt động đầy đủ, cần chạy qua HTTP server:

```bash
# Python
python3 -m http.server 8000

# Node.js (npx)
npx serve .

# VS Code
# Cài extension "Live Server", click "Go Live"
```

Sau đó mở `http://localhost:8000`

### Cài đặt PWA
Khi truy cập qua HTTPS hoặc localhost, trình duyệt sẽ hiện banner "Cài đặt ứng dụng". Nhấn **Cài đặt** để thêm vào màn hình chính.

---

## Công thức tính BMI

```
BMI = Cân nặng (kg) ÷ [Chiều cao (m)]²
```

**Phân loại theo WHO:**

| Phân loại               | BMI           |
|-------------------------|---------------|
| Thiếu cân nghiêm trọng  | < 16          |
| Thiếu cân               | 16 – 18.5     |
| Bình thường             | 18.5 – 25     |
| Thừa cân                | 25 – 30       |
| Béo phì độ I            | 30 – 35       |
| Béo phì độ II           | 35 – 40       |
| Béo phì độ III          | ≥ 40          |

---

## Công nghệ sử dụng

| Công nghệ             | Vai trò                              |
|-----------------------|--------------------------------------|
| HTML5                 | Cấu trúc                             |
| CSS3 (Custom Props)   | Giao diện, theming, responsive       |
| Vanilla JavaScript    | Logic, state, i18n, localStorage     |
| Material Icons Round  | Biểu tượng (Google Fonts)            |
| Be Vietnam Pro        | Font chữ (hỗ trợ tiếng Việt)         |
| Web App Manifest      | PWA metadata                         |
| Service Worker        | Cache offline                        |
| cairosvg + Pillow     | Tạo icon PNG từ SVG                  |

---

## Trình duyệt hỗ trợ

| Trình duyệt | Hỗ trợ |
|-------------|--------|
| Chrome 90+  | ✅     |
| Firefox 88+ | ✅     |
| Safari 14+  | ✅     |
| Edge 90+    | ✅     |
| Samsung Internet | ✅ |

---

## Lưu ý

> BMI chỉ mang tính chất tham khảo và không thay thế chẩn đoán y tế chuyên nghiệp. Hãy tham khảo bác sĩ để được tư vấn chính xác.

---

## Giấy phép

MIT License — Tự do sử dụng, chỉnh sửa, và phân phối.
