# Wedding Invitation - Tài & Huyền

Website thiệp cưới cho Tài & Huyền.

## Cấu trúc

- `index.html` - Trang chính (Nhà Gái) - 10/01/2026
- `index-nha-trai.html` - Trang Nhà Trai - 11/01/2026

## Deploy lên Vercel

### Cách 1: Deploy qua Vercel CLI (Khuyến nghị)

1. **Cài đặt Vercel CLI** (nếu chưa có):
   ```bash
   npm install -g vercel
   ```

2. **Đăng nhập vào Vercel**:
   ```bash
   vercel login
   ```

3. **Deploy project**:
   ```bash
   vercel
   ```
   
   - Lần đầu tiên sẽ hỏi một số câu hỏi:
     - Set up and deploy? → **Y**
     - Which scope? → Chọn tài khoản của bạn
     - Link to existing project? → **N**
     - Project name? → Nhập tên project (ví dụ: `wedding-invitation`)
     - Directory? → **./** (Enter)
     - Override settings? → **N**

4. **Deploy production**:
   ```bash
   vercel --prod
   ```

### Cách 2: Deploy qua GitHub

1. **Tạo repository trên GitHub**:
   - Tạo repo mới trên GitHub
   - Push code lên GitHub:
     ```bash
     git init
     git add .
     git commit -m "Initial commit"
     git branch -M main
     git remote add origin <your-github-repo-url>
     git push -u origin main
     ```

2. **Kết nối với Vercel**:
   - Vào [vercel.com](https://vercel.com)
   - Đăng nhập và chọn "Add New Project"
   - Import repository từ GitHub
   - Vercel sẽ tự động detect và deploy

### Cách 3: Deploy trực tiếp qua Vercel Dashboard

1. Vào [vercel.com](https://vercel.com)
2. Chọn "Add New Project"
3. Upload thư mục project hoặc kéo thả
4. Vercel sẽ tự động deploy

## URLs sau khi deploy

Sau khi deploy thành công, bạn sẽ có:

- **Trang chính (Nhà Gái)**: `https://your-project.vercel.app/`
- **Trang Nhà Trai**: `https://your-project.vercel.app/nha-trai` hoặc `https://your-project.vercel.app/index-nha-trai.html`

## Lưu ý

- Đảm bảo tất cả file ảnh trong thư mục `images/` đã được commit
- File `vercel.json` đã được cấu hình để routing đúng
- Nếu cần update, chỉ cần chạy lại `vercel --prod` hoặc push code mới lên GitHub

