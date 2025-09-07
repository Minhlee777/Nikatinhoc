# Hướng dẫn thêm tên miền cá nhân cho website

## Bước 1: Mua tên miền

### Các nhà cung cấp tên miền phổ biến tại Việt Nam:
- **Tenten.vn** - Nhà cung cấp lớn nhất VN
- **INET.vn** - Giá cả hợp lý
- **GoDaddy** - Quốc tế, nhiều tùy chọn
- **Namecheap** - Giá rẻ, dễ sử dụng

### Cách chọn tên miền:
- Ngắn gọn, dễ nhớ
- Liên quan đến nội dung website
- Tránh dấu gạch ngang
- Ưu tiên .com, .vn, .net

## Bước 2: Chọn dịch vụ hosting

### Hosting miễn phí (Khuyến nghị cho website tĩnh):

#### GitHub Pages (Miễn phí)
1. Tạo tài khoản GitHub
2. Tạo repository mới
3. Upload các file website
4. Bật GitHub Pages trong Settings
5. Website sẽ có địa chỉ: `username.github.io/repository-name`

#### Netlify (Miễn phí)
1. Đăng ký tài khoản Netlify
2. Kéo thả thư mục website vào Netlify
3. Website sẽ có địa chỉ: `random-name.netlify.app`

#### Vercel (Miễn phí)
1. Đăng ký tài khoản Vercel
2. Import project từ GitHub
3. Deploy tự động

### Hosting trả phí:
- **Hostinger** - Giá rẻ, tốc độ nhanh
- **iPage** - Dễ sử dụng
- **Bluehost** - Chuyên nghiệp

## Bước 3: Kết nối tên miền với hosting

### Với GitHub Pages:
1. Vào Settings của repository
2. Tìm phần "Custom domain"
3. Nhập tên miền của bạn
4. Tạo file `CNAME` trong repository với nội dung là tên miền

### Với Netlify:
1. Vào Site settings
2. Chọn "Domain management"
3. Thêm custom domain
4. Làm theo hướng dẫn DNS

### Với Vercel:
1. Vào Project settings
2. Chọn "Domains"
3. Thêm domain
4. Cấu hình DNS

## Bước 4: Cấu hình DNS

### Các bản ghi DNS cần thiết:

#### Cho GitHub Pages:
```
Type: CNAME
Name: www
Value: username.github.io
```

#### Cho Netlify:
```
Type: CNAME
Name: www
Value: your-site.netlify.app
```

#### Cho Vercel:
```
Type: CNAME
Name: www
Value: cname.vercel-dns.com
```

### Redirect tên miền chính:
```
Type: A
Name: @
Value: [IP của hosting]
```

## Bước 5: Chờ DNS propagate
- Thời gian: 24-48 giờ
- Kiểm tra bằng: whatsmydns.net

## Bước 6: Cài đặt SSL Certificate
- Hầu hết hosting miễn phí đều tự động cài SSL
- Đảm bảo website chạy với HTTPS

## Lưu ý quan trọng:

1. **Backup website** trước khi upload
2. **Kiểm tra tất cả link** hoạt động đúng
3. **Test trên nhiều thiết bị** khác nhau
4. **Cập nhật thông tin liên hệ** trong website
5. **Thiết lập Google Analytics** để theo dõi

## Chi phí ước tính:
- Tên miền .com: ~$10-15/năm
- Tên miền .vn: ~300,000-500,000 VNĐ/năm
- Hosting miễn phí: $0
- Hosting trả phí: $3-10/tháng

## Hỗ trợ kỹ thuật:
- Liên hệ nhà cung cấp tên miền
- Hỗ trợ từ hosting provider
- Tài liệu hướng dẫn online
