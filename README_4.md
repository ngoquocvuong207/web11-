# Editor 3: Form nhập URL giả lập

## Mô tả

Trang HTML có form cho phép người dùng nhập một URL bất kỳ, nhấn nút **Phân tích URL** để hiển thị bảng kết quả gồm 5 thành phần: Protocol, Domain, Path, Query, Fragment.

## Cấu trúc file

```
project/
└── index.html
```

## Tính năng

- Input có placeholder gợi ý URL mẫu
- Nhấn button hoặc nhấn **Enter** để phân tích
- Dùng JavaScript `new URL()` để parse URL thực sự
- Hiển thị kết quả dạng bảng với màu sắc từng thành phần
- Báo lỗi nếu URL nhập vào không hợp lệ

## Cách chạy

1. Lưu file `index.html` về máy
2. Mở bằng trình duyệt (nhấp đôi hoặc kéo vào Chrome/Firefox)
3. Nhập URL vào ô input, nhấn **Phân tích URL**
4. Hoặc dán nội dung vào [CodePen](https://codepen.io) để chạy online

## Ví dụ sử dụng

Nhập vào: `https://example.com/products/list?page=2#top`

| Thành phần | Giá trị |
|---|---|
| Protocol | `https:` |
| Domain | `example.com` |
| Path | `/products/list` |
| Query | `?page=2` |
| Fragment | `#top` |

## Đẩy lên GitHub Pages

```bash
# 1. Tạo repo mới (ví dụ: url-form)
git clone https://github.com/<username>/url-form.git

# 2. Copy file index.html vào thư mục repo
git add index.html
git commit -m "Add URL input form"
git push origin main

# 3. Vào Settings > Pages > branch main, thư mục root > Save
# Link: https://<username>.github.io/url-form/
```

## Yêu cầu đã đáp ứng

- [x] Có `<input>` với placeholder nhập URL
- [x] Có `<button>` Phân tích URL
- [x] Có `<script>` xử lý tương tác
- [x] Parse và hiển thị đủ 5 thành phần URL
- [x] Xử lý lỗi khi URL không hợp lệ
