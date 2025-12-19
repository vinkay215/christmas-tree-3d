# 🎄 Cây Giáng Sinh 3D Cao Cấp - Vinkay

[![Tác giả](https://img.shields.io/badge/Tác%20giả-vinkay215-blue)](https://github.com/vinkay215)
[![Ngày tạo](https://img.shields.io/badge/Ngày-06%2F08%2F2025-green)]()

Chào mừng đến với dự án **Cây Giáng Sinh 3D Cao Cấp**! Đây là một dự án tương tác 3D được tạo ra để chào mừng Giáng Sinh. ✨

Dự án này không chỉ là một cây thông Noel tĩnh thông thường, mà là một cây thông được tạo từ **hàng nghìn hạt 3D** với khả năng nhận diện cử chỉ tay AI, cho phép bạn điều khiển cây thông bằng tay và treo những bức ảnh kỷ niệm của mình lên cây.

## 🌐 Xem Demo Trực Tuyến

Bạn có thể xem và trải nghiệm dự án trực tuyến tại: **[https://christmas-vinkay.vercel.app/](https://christmas-vinkay.vercel.app/)**

⚠️ **Lưu ý quan trọng:**
- **Yêu cầu cấp quyền camera**: Để sử dụng tính năng điều khiển cử chỉ tay AI, bạn cần cho phép trình duyệt truy cập camera khi được yêu cầu
- **Nếu gặp lỗi**: Hãy thử reload lại trang (F5 hoặc Ctrl+R) và cho phép quyền camera
- **HTTPS**: Dự án đã được deploy trên HTTPS, đảm bảo camera hoạt động tốt

---

## 🌟 Giới thiệu

Đây là một dự án web tương tác 3D sử dụng **Three.js** và **MediaPipe** để tạo ra một cây thông Noel đẹp mắt với các tính năng:

* **Hiệu ứng hạt 3D**: Cây thông được tạo từ hàng nghìn hạt, có thể xoay, thở và phân tán thành vô số ngôi sao
* **Điều khiển cử chỉ tay AI**: Không cần chuột, chỉ cần đưa tay vào camera để điều khiển cây thông
* **Treo ảnh kỷ niệm**: Upload ảnh của bạn, chúng sẽ được đóng khung vàng và treo quanh cây
* **Giao diện sang trọng**: Thiết kế tối giản với tông màu đen vàng, tạo cảm giác cao cấp

---

## 📁 Danh sách các phiên bản

Dự án bao gồm **8 phiên bản** khác nhau, mỗi phiên bản có tính năng riêng:

### 1. `tree_basic.html` - Phiên Bản Cơ Bản
**Chức năng:**
- Cây thông 3D với các hạt trang trí (hộp xanh, hộp vàng, quả cầu vàng, quả cầu đỏ, kẹo gậy)
- Upload ảnh đơn giản qua nút "Add Memories"
- Điều khiển cử chỉ tay AI (nắm tay, duỗi tay, nắm)
- Hiệu ứng bloom và ánh sáng đẹp mắt
- Ngôi sao 8 cạnh ở đỉnh cây

**Cách hoạt động:**
- Mở file và cho phép truy cập camera
- Upload ảnh qua nút ở góc trên bên phải
- Sử dụng cử chỉ tay để điều khiển: nắm tay = cây, duỗi tay = phân tán, nắm = focus ảnh

---

### 2. `tree_cloud.html` - Phiên Bản Hỗ Trợ Ảnh Đám Mây
**Chức năng:**
- Tất cả tính năng của phiên bản cơ bản
- **Tải ảnh từ URL đám mây** - Bạn có thể thêm link ảnh trực tiếp vào code
- Hỗ trợ cảm ứng đa điểm (kéo để xoay, chạm để chọn ảnh)
- Hiệu ứng tuyết rơi
- Nút chuyển đổi chế độ ở dưới màn hình (Cây / Phân tán / Focus)

**Cách hoạt động:**
- Mở file và chỉnh sửa mảng `cloudImageUrls` trong phần CONFIG để thêm link ảnh
- Ảnh sẽ tự động tải từ các URL bạn cung cấp
- Có thể upload thêm ảnh local nếu cần
- Nhấn phím 'H' để ẩn/hiện điều khiển

---

### 3. `tree_folder.html` - Phiên Bản Tự Động Đọc Thư Mục
**Chức năng:**
- Tất cả tính năng của phiên bản cơ bản
- **Upload cả thư mục** - Chọn một thư mục và tất cả ảnh sẽ được tải tự động
- **Quét tự động thư mục `./images/`** - Tự động tải ảnh từ thư mục local (1.jpg, 2.jpg, ...)
- Bố cục ảnh xoắn ốc quanh cây
- Hỗ trợ cả JPG và PNG

**Cách hoạt động:**
- Đặt ảnh vào thư mục `./images/` với tên `(1).jpg`, `(2).jpg`, ... (tối đa 200 ảnh)
- Hoặc sử dụng nút "Select Folder" để chọn thư mục bất kỳ
- Ảnh sẽ được tự động sắp xếp theo hình xoắn ốc quanh cây

---

### 4. `tree_helical.html` - Phiên Bản Xoắn Ốc
**Chức năng:**
- Tất cả tính năng của phiên bản cơ bản
- **Bố cục ảnh xoắn ốc đẹp mắt** - Ảnh được sắp xếp theo hình xoắn ốc 3 vòng quanh cây
- Ảnh luôn hướng ra ngoài để dễ xem
- Ngôi sao 5 cánh ở đỉnh cây (thay vì 8 cạnh)
- Tự động tính toán lại bố cục khi thêm ảnh mới

**Cách hoạt động:**
- Upload ảnh và chúng sẽ tự động được sắp xếp theo hình xoắn ốc
- Mỗi ảnh được đặt ở vị trí phù hợp dựa trên số lượng ảnh
- Ảnh luôn hướng về camera để dễ xem nhất

---

### 5. `tree_pro.html` - Phiên Bản Chuyên Nghiệp
**Chức năng:**
- Tất cả tính năng của phiên bản cơ bản
- **Hiệu ứng tuyết rơi** - 1000 bông tuyết rơi liên tục
- Nền gradient màu xanh đêm thay vì đen thuần túy
- Ánh sáng được tối ưu để tạo cảm giác ánh trăng
- Upload thư mục và quét tự động
- Hệ thống nhận diện cử chỉ tay được tối ưu (sử dụng tỷ lệ tương đối)

**Cách hoạt động:**
- Tự động hiển thị tuyết rơi khi mở file
- Nền gradient tạo không gian sâu hơn
- Cử chỉ tay hoạt động chính xác hơn nhờ thuật toán tối ưu

---

### 6. `tree_star.html` - Phiên Bản Cử Chỉ Tay Thích Ứng
**Chức năng:**
- Tất cả tính năng của phiên bản cơ bản
- **Hệ thống nhận diện cử chỉ tay thông minh** - Sử dụng tỷ lệ tương đối thay vì khoảng cách tuyệt đối
- Hoạt động tốt với mọi kích thước bàn tay và khoảng cách camera
- Upload thư mục và quét tự động
- Bố cục ảnh xoắn ốc
- Hiển thị thông tin debug về cử chỉ tay

**Cách hoạt động:**
- Hệ thống tự động điều chỉnh theo kích thước bàn tay của bạn
- Không cần phải đứng ở khoảng cách cố định
- Hiển thị thông tin debug ở góc dưới để theo dõi cử chỉ

---

### 7. `tree_touch.html` - Phiên Bản Cảm Ứng & Thống Kê
**Chức năng:**
- Tất cả tính năng của phiên bản chuyên nghiệp
- **Hỗ trợ cảm ứng đa điểm** - Kéo để xoay, chạm để chọn ảnh, double-tap để chuyển chế độ
- **Bảng thống kê người truy cập** - Hiển thị số lượt xem và số người truy cập (ẩn mặc định, nhấn 'S' để hiện)
- Bản đồ hiển thị vị trí người truy cập trên thế giới
- Tích hợp FontAwesome icons
- Tích hợp script đếm lượt truy cập (不蒜子)

**Cách hoạt động:**
- Trên mobile: Kéo để xoay, chạm ảnh để xem, double-tap để chuyển chế độ
- Trên desktop: Kéo chuột để xoay, click ảnh để xem
- Nhấn phím 'S' để hiện/ẩn bảng thống kê
- Nhấn phím 'H' để ẩn/hiện điều khiển

---

### 8. `tree_wp.html` - Phiên Bản WP
**Chức năng:**
- Phiên bản đơn giản với ảnh mặc định có chữ "WISH U HAPPY WP :)"
- Upload ảnh đơn giản
- Điều khiển cử chỉ tay AI
- Ngôi sao 8 cạnh ở đỉnh cây
- Giao diện tối giản nhất

**Cách hoạt động:**
- Mở file sẽ thấy ảnh mặc định với lời chúc
- Upload ảnh để thay thế hoặc thêm vào
- Sử dụng cử chỉ tay để điều khiển

---

## 🛠️ Công nghệ sử dụng

Dự án sử dụng các công nghệ web hiện đại:

* **Three.js v0.160.0** - Thư viện 3D JavaScript, xử lý rendering, camera, ánh sáng, và hiệu ứng bloom
* **MediaPipe Tasks Vision v0.10.3** - AI nhận diện cử chỉ tay của Google, phát hiện và phân tích cử chỉ trong thời gian thực
* **ES Modules** - Sử dụng import/export để tổ chức code
* **HTML5 Canvas & WebGL** - Rendering 3D hiệu suất cao
* **FontAwesome 6.0.0** - Icons đẹp cho bảng thống kê
* **不蒜子 (Busuanzi)** - Script đếm lượt truy cập (chỉ trong tree_touch.html)

---

## 🎮 Hướng dẫn sử dụng

### 🖐️ Điều khiển bằng cử chỉ tay (Quan trọng!)

**Yêu cầu:** Cho phép trình duyệt truy cập camera

1. **Nắm tay (✊)**: Chế độ Cây - Tất cả hạt và ảnh quay về vị trí cây thông
2. **Duỗi tay (🖐️)**: Chế độ Phân tán - Hạt và ảnh bay ra xung quanh, bạn có thể xoay bằng cách di chuyển tay
3. **Nắm (🤏)**: Chế độ Focus - Một ảnh ngẫu nhiên sẽ được phóng to và hiển thị ở giữa màn hình

### 🖱️ Điều khiển bằng chuột/cảm ứng

* **Kéo**: Xoay cây thông
* **Click/Chạm ảnh**: Chuyển sang chế độ Focus để xem ảnh đó
* **Double-tap** (mobile): Chuyển đổi giữa chế độ Cây và Phân tán
* **Phím 'H'**: Ẩn/hiện tất cả điều khiển UI
* **Phím 'S'** (chỉ tree_touch.html): Ẩn/hiện bảng thống kê

### 📤 Upload ảnh

1. **Upload đơn**: Click nút "Add Memories" hoặc "Chọn File" và chọn một hoặc nhiều ảnh
2. **Upload thư mục**: Click "Select Folder" hoặc "Chọn Thư Mục" và chọn cả thư mục (chỉ một số phiên bản hỗ trợ)
3. **Tự động quét**: Đặt ảnh vào thư mục `./images/` với tên `(1).jpg`, `(2).jpg`, ... (chỉ một số phiên bản hỗ trợ)
4. **Ảnh đám mây**: Thêm link ảnh vào mảng `cloudImageUrls` trong code (chỉ tree_cloud.html)

---

## 🚀 Cách chạy dự án

⚠️ **Lưu ý quan trọng:** Vì dự án sử dụng ES Modules và cần quyền truy cập camera, **KHÔNG được mở trực tiếp file HTML bằng cách double-click**. Bạn phải chạy qua một local server.

### Cách 1: Sử dụng VS Code (Khuyến nghị)

1. Cài đặt extension **Live Server** trong VS Code
2. Click chuột phải vào file HTML bất kỳ
3. Chọn **"Open with Live Server"**

### Cách 2: Sử dụng Python

Mở terminal trong thư mục dự án và chạy:

```bash
python -m http.server 8000
```

Sau đó mở trình duyệt và truy cập: `http://localhost:8000`

### Cách 3: Sử dụng Node.js

```bash
npx http-server .
```

Sau đó mở trình duyệt và truy cập địa chỉ được hiển thị (thường là `http://localhost:8080`)

### Cách 4: Sử dụng PHP

```bash
php -S localhost:8000
```

---

## ☁️ Deploy lên Vercel

Dự án đã được cấu hình sẵn để deploy lên Vercel một cách dễ dàng. File `vercel.json` đã được tạo sẵn với các cấu hình cần thiết.

### Cách 1: Deploy qua Vercel CLI (Khuyến nghị)

1. **Cài đặt Vercel CLI** (nếu chưa có):
```bash
npm i -g vercel
```

2. **Đăng nhập vào Vercel**:
```bash
vercel login
```

3. **Deploy dự án**:
```bash
vercel
```

4. **Deploy lên production**:
```bash
vercel --prod
```

### Cách 2: Deploy qua GitHub

1. **Push code lên GitHub repository**
2. Vào [vercel.com](https://vercel.com) và đăng nhập
3. Click **"Add New Project"**
4. Import repository từ GitHub
5. Vercel sẽ tự động detect cấu hình và deploy

### Cách 3: Deploy qua Vercel Dashboard

1. Vào [vercel.com/new](https://vercel.com/new)
2. Kéo thả thư mục dự án vào hoặc chọn từ GitHub
3. Vercel sẽ tự động deploy

### Lưu ý khi deploy:

- ✅ **HTTPS tự động**: Vercel tự động cung cấp HTTPS, cần thiết cho camera API
- ✅ **Cấu hình sẵn**: File `vercel.json` đã được tạo với headers và rewrites phù hợp
- ✅ **Zero config**: Không cần cấu hình thêm, chỉ cần deploy là xong
- ⚠️ **Camera**: Đảm bảo cho phép camera trong trình duyệt khi sử dụng

### Sau khi deploy:

Sau khi deploy thành công, bạn sẽ nhận được một URL như: `https://your-project.vercel.app`

Truy cập các phiên bản:
- `https://your-project.vercel.app/` - Trang chủ
- `https://your-project.vercel.app/tree_basic.html` - Phiên bản cơ bản
- `https://your-project.vercel.app/tree_cloud.html` - Phiên bản đám mây
- ... và các phiên bản khác

---

## 📝 Tùy chỉnh

### Thêm ảnh đám mây (tree_cloud.html)

Mở file `tree_cloud.html` và tìm phần:

```javascript
cloudImageUrls: [
    // Thêm các link ảnh tại đây
],
```

Thêm link ảnh của bạn vào, ví dụ:

```javascript
cloudImageUrls: [
    'https://example.com/image1.jpg',
    'https://example.com/image2.png',
    'https://example.com/image3.webp',
],
```

### Thay đổi số lượng hạt

Tìm phần `CONFIG` và chỉnh sửa:

```javascript
particles: {
    count: 1500,      // Số hạt trang trí
    dustCount: 2000,  // Số hạt bụi lấp lánh
    snowCount: 1000,  // Số bông tuyết (nếu có)
    treeHeight: 24,  // Chiều cao cây
    treeRadius: 8     // Bán kính cây
}
```

### Thay đổi màu sắc

Tìm phần `colors` trong `CONFIG`:

```javascript
colors: {
    bg: 0x000000,           // Màu nền
    champagneGold: 0xffd966, // Màu vàng champagne
    deepGreen: 0x03180a,     // Màu xanh lá đậm
    accentRed: 0x990000,     // Màu đỏ nhấn
}
```

---

## 🎯 So sánh các phiên bản

| Phiên bản | Upload Ảnh | Cử chỉ tay | Cảm ứng | Tuyết | Thống kê | Bố cục |
|-----------|------------|------------|---------|-------|----------|--------|
| tree_basic.html | ✅ Đơn | ✅ | ❌ | ❌ | ❌ | Mặc định |
| tree_cloud.html | ✅ Đám mây + Local | ✅ | ✅ | ✅ | ❌ | Xoắn ốc |
| tree_folder.html | ✅ Thư mục + Auto | ✅ | ❌ | ❌ | ❌ | Xoắn ốc |
| tree_helical.html | ✅ Đơn | ✅ | ❌ | ❌ | ❌ | Xoắn ốc |
| tree_pro.html | ✅ Thư mục + Auto | ✅ | ❌ | ✅ | ❌ | Xoắn ốc |
| tree_star.html | ✅ Thư mục + Auto | ✅ Tối ưu | ❌ | ❌ | ❌ | Xoắn ốc |
| tree_touch.html | ✅ Thư mục + Auto | ✅ | ✅ | ✅ | ✅ | Xoắn ốc |
| tree_wp.html | ✅ Đơn | ✅ | ❌ | ❌ | ❌ | Mặc định |

---

## 🔧 Xử lý lỗi

### Camera không hoạt động

1. **Kiểm tra quyền truy cập**: Đảm bảo bạn đã cho phép trình duyệt truy cập camera
2. **HTTPS**: Camera chỉ hoạt động trên HTTPS hoặc localhost
3. **Trình duyệt**: Sử dụng Chrome, Edge hoặc Firefox mới nhất

### Ảnh không hiển thị

1. **Định dạng**: Chỉ hỗ trợ JPG, PNG, WEBP
2. **Kích thước**: Ảnh quá lớn có thể tải chậm
3. **Đường dẫn**: Kiểm tra đường dẫn ảnh nếu dùng local

### Hiệu suất thấp

1. **Giảm số lượng hạt**: Chỉnh `particles.count` xuống thấp hơn
2. **Tắt hiệu ứng tuyết**: Comment dòng `createSnow()` và `updateSnow()`
3. **Giảm độ phân giải**: Chỉnh `renderer.setPixelRatio()` xuống 1

---

## 📄 Thông tin dự án

- **Tác giả**: vinkay215
- **Ngày tạo**: 06/08/2025
- **Giấy phép**: Miễn phí sử dụng và chỉnh sửa
- **Ngôn ngữ**: Tiếng Việt
- **Donate**: [💝 Ủng hộ tác giả](https://vinkay.vercel.app)

---

## 🙏 Lời cảm ơn

Dự án này được phát triển dựa trên ý tưởng ban đầu và được cải tiến với nhiều tính năng mới. Cảm ơn tất cả những người đã đóng góp và sử dụng dự án này!

---

## 🎄 Chúc mừng Giáng Sinh!

Nếu bạn thích dự án này, hãy Star repo hoặc Fork để tùy chỉnh theo ý thích của bạn!

**Merry Christmas! 🎅✨**
