# Giai đoạn 3 — Character & Product Reference Sheets

## Mục đích
Khóa chặt diện mạo nhân vật (on-model) và đặc điểm bao bì sản phẩm (product consistency) ở tỷ lệ dọc 9:16 trước khi tạo video trên Muse AI.

---

## 1. Luật Khóa Tỷ Lệ (STRICT ASPECT RATIO LOCK)

Dán nguyên văn ràng buộc này vào mọi prompt tạo ảnh sheet và keyframe:
```text
STRICT ASPECT RATIO LOCK: The canvas MUST be exactly 9:16 vertical (720x1280 or 1080x1920). 
All character turnarounds, product model views, and keyframes share this vertical aspect ratio. 
Never produce horizontal 16:9 or square 1:1 references.
```

---

## 2. Character Reference Sheet (Khóa Nhân Vật)

Để nhân vật không bị đổi trang phục, màu tóc hoặc khuôn mặt giữa các cảnh:
* **Chi tiết cụ thể:** Đừng viết "chàng trai mặc áo thun". Phải viết: *"Chubby young office worker with messy black hair, round glasses, wearing a mint green polo shirt with white collar, beige khaki shorts, white sneakers"*.
* **Bố cục sheet dọc 9:16:** Sheet gồm 3 khung hình:
  * Khung trên: Mặt cận cảnh (biểu cảm hoảng hốt và biểu cảm thở phào).
  * Khung giữa: Toàn thân nhìn thẳng 3/4.
  * Khung dưới: Toàn thân góc nghiêng cạnh bên.

### Mẫu Prompt vẽ Character Sheet:
```text
3D stylized animation character model sheet, Pixar commercial style, 9:16 vertical orientation.
Character: [Tên nhân vật, tuổi tác, vóc dáng, chi tiết trang phục, màu sắc quần áo cố định].
Multiple angles on a clean solid gradient studio background: front 3/4 view, side profile view, 
and close-up facial expressions (panicked eyes wide open vs relieved satisfied smile).
Soft studio lighting, clean geometry, highly consistent design, no text, no watermark.
```

---

## 3. Product Reference Sheet (Khóa Sản Phẩm)

Sản phẩm là "ngôi sao thứ hai" của video bán hàng. Nếu qua mỗi cảnh cái bình đổi màu hoặc biến dạng thành cái cốc thì video thất bại.
* **Quy chuẩn Product Sheet:**
  * Khung trên: Góc chụp cận cảnh sản phẩm với nhãn hiệu/logo rõ nét.
  * Khung giữa: Cơ chế hoạt động (nắp mở ra sao, vòi xịt như thế nào, nút bấm đặt ở đâu).
  * Khung dưới: Tương quan kích thước khi bàn tay nhân vật cầm sản phẩm.

### Mẫu Prompt vẽ Product Sheet:
```text
Commercial product model sheet, 3D render style, 9:16 vertical aspect ratio.
Product: [Tên sản phẩm, mô tả hình học chai/lọ/hộp, màu sắc chính xác, chất liệu vỏ nhám hay bóng, vị trí nắp và nút bấm].
Three views on clean backdrop: isolated hero product angle, close-up of the mechanical cap/nozzle, 
and human stylized hand holding the product demonstrating correct scale and grip.
Crisp studio commercial lighting, ultra-consistent geometry, photorealistic yet stylized finish.
```

---

## 4. Thứ Tự Nạp Reference Khi Render Video Trên Muse AI

Khi render video từng cảnh (Giai đoạn 5), bắt buộc phải nạp ảnh theo đúng thứ tự ưu tiên:
1. `CHARACTER_SHEET_9_16.png` (Ref nhận diện nhân vật số 1)
2. `PRODUCT_SHEET_9_16.png` (Ref nhận diện sản phẩm số 2)
3. `KEYFRAME_START_SCENE.png` (Keyframe khung đầu của cảnh)
4. `KEYFRAME_END_SCENE.png` (Keyframe khung cuối để match-cut)
*Sau đó mới dán đoạn văn bản Mega Prompt.*
