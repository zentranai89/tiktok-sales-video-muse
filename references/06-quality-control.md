# Giai đoạn 6 — Kiểm Soát Chất Lượng (Quality Control)

## Mục đích
Phát hiện và loại bỏ các lỗi tạo hình, lỗi chuyển động AI và méo mó sản phẩm ngay khi nhận clip từ Muse AI. Tuyệt đối không chấp nhận clip lỗi vào khâu dựng.

---

## 1. Ma Trận Nghiệm Thu Clip Muse AI

Kiểm tra video render theo 6 tiêu chí:

| Hạng mục | Dấu hiệu lỗi (Phải loại bỏ & Làm lại) | Đạt chuẩn (Pass) |
| :--- | :--- | :--- |
| **1. Nhân vật** | Dị tật bàn tay (6 ngón, ngón dính chùm), mặt bị trôi sang nhân vật khác, đổi màu tóc/áo. | Giữ nguyên tỷ lệ cơ thể và trang phục đúng với Character Sheet. Bàn tay cử động tự nhiên. |
| **2. Sản phẩm** | Logo méo mó, hình dáng chai bị biến dạng (lúc tròn lúc vuông), nắp chai tự động bốc hơi. | Đúng chuẩn Product Sheet: dáng bao bì nguyên vẹn, màu sắc đồng nhất, cơ chế hoạt động rõ ràng. |
| **3. Chuyển động** | Vật thể đi xuyên qua người (clipping), vật lý lơ lửng vô trọng lực phi logic. | Chuyển động cơ học chắc chắn, có quán tính va chạm thực tế. |
| **4. Tỷ lệ & Khung hình** | Bị viền đen hai bên (pillarbox) hoặc bị giãn dẹt do render sai orientation. | Chuẩn khung hình dọc 9:16 (720×1280), chủ thể nằm trong vùng an toàn (Safe Zone) của TikTok. |
| **5. Tính liên tục** | Vị trí nhân vật ở đầu Cảnh 2 bị nhảy cóc so với cuối Cảnh 1. | Match-cut liền mạch: vị trí tay và hướng nhìn giữa hai cảnh ăn khớp nhau. |
| **6. Biểu cảm & Cảm xúc** | Biểu cảm đơ cứng vô hồn, không toát lên được sự hài hước hoặc cú sốc. | Biểu cảm sống động, phóng đại nhẹ theo phong cách phim hoạt hình thương mại. |

---

## 2. Quy Tắc Sửa Prompt Thay Vì Cố Chấp Generate Lại

* Nếu một cảnh bị lỗi liên tiếp **2 lần**, vấn đề 95% nằm ở **Mega Prompt**:
  * *Hành động quá phức tạp:* Chia nhỏ động tác hoặc giảm bớt chi tiết thừa.
  * *Prompt viết từ mơ hồ:* Thay thế động từ trừu tượng bằng động từ cơ học cụ thể.
  * *Lệch sản phẩm:* Kiểm tra xem Product Sheet có bị nạp sai thứ tự sau Keyframe không. Đưa Product Sheet lên trước.
