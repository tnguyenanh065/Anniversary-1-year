# Ngân Keychain

Trang xem trước móc khoá mica: khách tải ảnh lên, chọn hình, kích thước, loại móc và lưu ảnh móc khoá.
Toàn bộ trang nằm trong một file `index.html`, không cần cài đặt hay máy chủ riêng.

## Đưa lên GitHub Pages (miễn phí)

1. Tạo repository mới trên GitHub, đặt tên ví dụ `ngan-keychain`, chọn **Public**.
2. Đẩy các file trong thư mục này lên nhánh `main`:
   ```bash
   git init
   git add .
   git commit -m "Ngân Keychain"
   git branch -M main
   git remote add origin https://github.com/<ten-tai-khoan>/ngan-keychain.git
   git push -u origin main
   ```
   Hoặc trên trang repository, bấm **Add file → Upload files** rồi kéo các file vào.
3. Vào **Settings → Pages**. Ở mục **Source** chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, bấm **Save**.
4. Đợi 1–2 phút, trang chạy tại `https://<ten-tai-khoan>.github.io/ngan-keychain/`.

## Gắn tên miền riêng (keychain.maxmuffin.com)

1. Ở nơi quản lý tên miền maxmuffin.com, tạo bản ghi **CNAME**: tên `keychain`, giá trị `<ten-tai-khoan>.github.io`.
2. Trong **Settings → Pages → Custom domain** của repository, nhập `keychain.maxmuffin.com`, bấm **Save**.
3. Khi GitHub báo kiểm tra DNS thành công, bật **Enforce HTTPS**.

## Cập nhật trang

Thay file `index.html` bằng bản mới rồi đẩy lên lại (hoặc Upload files đè lên). Trang tự cập nhật sau 1–2 phút.
Danh sách móc nằm sẵn trong `index.html`; muốn thêm hoặc sửa móc thì sửa trên bản trong Claude rồi xuất lại file này.
