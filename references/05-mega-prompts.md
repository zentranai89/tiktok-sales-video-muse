# Giai đoạn 5 — Bộ Mega Prompts Muse AI Chuẩn Hóa

## Mục đích
Cung cấp định dạng Mega Prompt tiếng Anh "copy-paste là chạy" cho từng cảnh trên Muse AI. Tích hợp đầy đủ Global Locks, Character Lock, Product Lock, Luật Realism và các chỉ dẫn camera/âm thanh.

---

## 1. Cấu Trúc Mega Prompt Hoàn Chỉnh

```text
[GLOBAL LOCKS]
Modern 3D stylized animation, Pixar commercial lighting and aesthetic, clean vibrant colors, 
vertical 9:16 aspect ratio (720x1280), commercial quality, no text, no watermark, no logos on clothing.
STRICT ASPECT RATIO LOCK: Exactly 9:16 vertical orientation. All visual elements framed for mobile screen.
CHARACTER LOCK: [Mô tả chi tiết ngoại hình nhân vật từ Character Sheet]. Keep character strictly on-model.
PRODUCT LOCK: [Mô tả chi tiết hình dáng, màu sắc, cơ chế của sản phẩm từ Product Sheet]. Keep product strictly on-model.

FIRST FRAME: [Mô tả chính xác khung hình đầu tiên của cảnh = Keyframe xuất phát, tỷ lệ 9:16].
MOTION: [Mô tả tuần tự diễn biến hành động từ giây 0 đến giây 10. Tuân thủ luật Realism cơ học].
CAMERA: [Chuyển động máy quay dọc: push-in, whip pan, tilt up, handheld tracking...].
LAST FRAME: match [Mô tả khung hình kết thúc cảnh để chuẩn bị match-cut sang cảnh sau].
SOUND: [Chi tiết hiệu ứng âm thanh SFX: tiếng va đập, tiếng mở nắp, tiếng rít, tiếng gió...].
MUSIC: [Diễn biến điệu nhạc: upbeat tempo, comedic pause, dramatic brass sting...].
VO (warm comedic narrator): "[Câu thoại tiếng Việt hoặc tiếng Anh, chiếm tối đa 60% thời lượng]".
```

---

## 2. ⚠️ Luật Realism Khi Viết MOTION (Bài Học Sống Còn)

Không bao giờ dùng những từ ngữ trừu tượng hoặc hành động vi phạm cơ chế vật lý:
* ❌ **Sai:** *"Anh ấy dùng sản phẩm và mọi vết ố biến mất kỳ diệu."*  
  👉 Muse AI sẽ tự biến hóa ra khói ma thuật hoặc làm dị tật bàn tay.
* ✅ **Đúng:** *"Tay nhân vật cầm bình xịt hướng vòi vào vết cà phê trên áo -> ngón trỏ nhấn cò xịt 2 lần tạo ra lớp bọt trắng mịn -> dùng khăn lau 1 đường ngang -> vết ố bị cuốn trôi để lại vải sạch tinh."*

### Bảng Kiểm Tra Động Từ Thực Tế:
| Hành động sản phẩm | Chuỗi diễn hoạt vật lý thực tế cần miêu tả |
| :--- | :--- |
| **Bình nước chống tràn** | Bàn tay vô tình gạt trúng thân bình -> bình ngã lăn tròn trên mặt bàn gỗ -> nắp chốt nhựa khóa chặt -> không có giọt nước nào bắn ra ngoài. |
| **Xịt thơm miệng / Khử mùi** | Mở nắp chụp bằng ngón cái -> đưa vòi xịt cách miệng 5cm -> ấn 1 nhịp xịt tia sương mịn -> khép miệng mỉm cười tự tin tỏa sáng. |
| **Kem dưỡng da / Chống nắng** | Mở nắp tuýp xoay -> bóp nhẹ thân tuýp cho hạt kem cỡ hạt đậu ra đầu ngón tay -> chấm lên má và thoa đều theo chuyển động xoay tròn. |

---

## 3. Checklist Trước Khi Bấm Generate

- [ ] Đã đính kèm đủ Reference files theo thứ tự: `Character Sheet` -> `Product Sheet` -> `Keyframe`?
- [ ] Tỷ lệ đã được khóa 9:16 trong cả prompt lẫn ảnh đính kèm chưa?
- [ ] Hành động trong `MOTION` có quá tải không? (Một clip 10 giây chỉ nên có từ 1 đến 2 hành động cơ học rõ ràng).
- [ ] Lời thoại VO có ngắn gọn, để lại khoảng lặng cho âm thanh thực tế không?
