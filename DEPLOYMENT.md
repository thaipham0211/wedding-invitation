# 🚀 Hướng dẫn Deploy Thiệp Cưới lên GitHub Pages

## Bước 1: Tạo Repository trên GitHub

1. Đăng nhập vào [GitHub](https://github.com)
2. Click nút **"New"** để tạo repository mới
3. Đặt tên repository (ví dụ: `wedding-invitation`)
4. Chọn **Public** (bắt buộc để sử dụng GitHub Pages miễn phí)
5. **KHÔNG** tích vào "Add a README file" (vì đã có sẵn)
6. Click **"Create repository"**

## Bước 2: Upload code lên GitHub

### Cách 1: Sử dụng Git Command Line

```bash
# Mở Terminal/Command Prompt tại thư mục dự án
cd wedding-invitation

# Khởi tạo Git repository
git init

# Thêm tất cả files
git add .

# Commit đầu tiên
git commit -m "Thêm thiệp cưới website"

# Thêm remote repository (thay YOUR_USERNAME bằng username GitHub của bạn)
git remote add origin https://github.com/YOUR_USERNAME/wedding-invitation.git

# Đặt tên branch chính
git branch -M main

# Push code lên GitHub
git push -u origin main
```

### Cách 2: Upload trực tiếp qua GitHub Web

1. Vào repository vừa tạo trên GitHub
2. Click **"uploading an existing file"**
3. Kéo thả tất cả files và folders vào
4. Viết commit message: "Thêm thiệp cưới website"
5. Click **"Commit changes"**

## Bước 3: Kích hoạt GitHub Pages

1. Vào repository trên GitHub
2. Click tab **"Settings"**
3. Cuộn xuống phần **"Pages"** ở sidebar bên trái
4. Trong phần **"Source"**:
   - Chọn **"Deploy from a branch"**
   - Branch: chọn **"main"**
   - Folder: chọn **"/ (root)"**
5. Click **"Save"**

## Bước 4: Truy cập website

- GitHub sẽ build và deploy website (có thể mất 5-10 phút)
- Website sẽ có địa chỉ: `https://YOUR_USERNAME.github.io/wedding-invitation`
- Bạn sẽ thấy link này trong phần Pages settings

## Bước 5: Custom Domain (Tùy chọn)

Nếu bạn có domain riêng:

1. Trong phần Pages settings
2. Thêm domain vào **"Custom domain"**
3. Tạo file `CNAME` trong root directory với nội dung là domain của bạn
4. Cấu hình DNS tại nhà cung cấp domain

## 🔄 Cập nhật website

Mỗi khi muốn cập nhật:

```bash
# Thêm changes
git add .

# Commit với message mô tả thay đổi
git commit -m "Cập nhật thông tin cưới"

# Push lên GitHub
git push
```

Website sẽ tự động cập nhật sau vài phút!

## ✅ Checklist

- [ ] Tạo GitHub repository
- [ ] Upload code
- [ ] Kích hoạt GitHub Pages
- [ ] Kiểm tra website hoạt động
- [ ] Chia sẻ link cho khách mời

## 🎯 Tips

- **Miễn phí 100%**: GitHub Pages hoàn toàn miễn phí
- **HTTPS tự động**: Website có SSL certificate
- **CDN toàn cầu**: Tốc độ tải nhanh worldwide
- **Responsive**: Website hoạt động tốt trên mọi thiết bị

## 🆘 Troubleshooting

### Website không hiển thị
- Kiểm tra repository có public không
- Đảm bảo file `index.html` ở root directory
- Chờ 10-15 phút sau khi enable Pages

### Ảnh không hiển thị
- Kiểm tra đường dẫn ảnh trong code
- Đảm bảo folder `images/` đã được upload
- Kiểm tra tên file có đúng case-sensitive không

### 404 Error
- Kiểm tra GitHub Pages settings
- Đảm bảo branch và folder được chọn đúng
- Refresh lại page sau vài phút

## 📞 Hỗ trợ

Nếu gặp khó khăn, bạn có thể:
1. Kiểm tra GitHub Pages documentation
2. Xem GitHub Actions tab để debug
3. Hỏi trên GitHub Community

---

**Chúc mừng! Thiệp cưới của bạn đã online! 🎉**
