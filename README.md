# Website Cá Nhân

Website tĩnh với thiết kế hiện đại, responsive và tối ưu SEO.

## Tính năng

- ✅ Responsive design
- ✅ Smooth scrolling
- ✅ Contact form
- ✅ Mobile navigation
- ✅ Loading animations
- ✅ SEO optimized

## Cách deploy

### GitHub Pages
1. Tạo repository mới trên GitHub
2. Upload tất cả files vào repository
3. Vào Settings > Pages
4. Chọn source: Deploy from a branch
5. Chọn branch: main
6. Website sẽ có địa chỉ: `username.github.io/repository-name`

### Netlify
1. Đăng ký tài khoản Netlify
2. Kéo thả thư mục website vào Netlify
3. Website sẽ có địa chỉ: `random-name.netlify.app`

### Vercel
1. Đăng ký tài khoản Vercel
2. Import project từ GitHub
3. Deploy tự động

## Cấu hình tên miền

### GitHub Pages
1. Tạo file `CNAME` với nội dung là tên miền của bạn
2. Cấu hình DNS:
   ```
   Type: CNAME
   Name: www
   Value: username.github.io
   ```

### Netlify
1. Vào Site settings > Domain management
2. Thêm custom domain
3. Cấu hình DNS theo hướng dẫn

### Vercel
1. Vào Project settings > Domains
2. Thêm domain
3. Cấu hình DNS

## Cấu trúc file

```
website/
├── index.html          # Trang chủ
├── styles.css          # CSS styles
├── script.js           # JavaScript
├── CNAME              # Tên miền cho GitHub Pages
├── _redirects         # Redirect cho Netlify
├── vercel.json        # Cấu hình cho Vercel
└── README.md          # Hướng dẫn
```

## Tùy chỉnh

### Thay đổi thông tin liên hệ
Chỉnh sửa trong file `index.html`:
- Địa chỉ (dòng 157)
- Số điện thoại (dòng 166)
- Email (dòng 175)

### Thay đổi màu sắc
Chỉnh sửa trong file `styles.css`:
- Màu chính: `#6366f1`
- Màu phụ: `#8b5cf6`

### Thêm nội dung
- Thêm section mới trong `index.html`
- Thêm styles tương ứng trong `styles.css`
- Thêm JavaScript nếu cần trong `script.js`

## Hỗ trợ

Nếu gặp vấn đề, hãy kiểm tra:
1. Tất cả files đã được upload đúng
2. Cấu hình DNS đã chính xác
3. SSL certificate đã được cài đặt
4. Website đã được test trên nhiều thiết bị

## License

MIT License - Sử dụng tự do cho mục đích cá nhân và thương mại.
