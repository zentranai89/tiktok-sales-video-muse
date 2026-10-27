# Giai đoạn 7 & 8 — Hậu Kỳ, Dựng Phim & Đo Lường Tối Ưu Chuyển Đổi

## Mục đích
Lắp ráp các clip thành phẩm thành video hoàn chỉnh trên CapCut hoặc FFmpeg, tối ưu nhịp dựng, hiệu ứng âm thanh, phụ đề động TikTok, và theo dõi các chỉ số chuyển đổi thương mại sau khi đăng tải.

---

## 1. Quy Chuẩn Kỹ Thuật Khi Dựng Phim

* **Độ phân giải:** 720×1280 hoặc 1080×1920 (9:16 dọc).
* **Frame rate:** 24fps hoặc 30fps đồng nhất.
* **FFmpeg lệnh chuẩn hóa trước khi nối (Normalize):**
  ```bash
  ffmpeg -i input_scene1.mp4 -vf "scale=720:1280:force_original_aspect_ratio=decrease,pad=720:1280:(ow-iw)/2:(oh-ih)/2,fps=24" -c:v libx264 -crf 20 -c:a aac scene1_normalized.mp4
  ```

---

## 2. Kỹ Thuật Dựng Giữ Chân (Pacing & Audio)

1. **J-Cut / L-Cut âm thanh:** Âm thanh của cảnh sau (tiếng va đập, tiếng la hét) vang lên trước 0.5 giây trước khi hình ảnh chuyển cảnh.
2. **Audio Ducking:** Khi giọng đọc thuyết minh (VO) cất lên, nhạc nền tự động hạ âm lượng xuống -15dB đến -18dB để lời thoại nổi bật rõ ràng.
3. **Hiệu ứng kịch tính tại cú Twist:** Ngắt toàn bộ nhạc nền trong 1–1.5 giây đúng thời điểm twist diễn ra, chỉ để lại tiếng thở dài hoặc tiếng SFX vui nhộn (cricket chirping, record scratch).
4. **Phụ đề động (Dynamic Captions):** Dùng font chữ đậm, nổi bật (trắng viền đen hoặc vàng) đặt ở trung tâm màn hình (vùng an toàn, tránh bị che bởi nút Like/Share bên phải và phần Caption bên dưới).

---

## 3. Tiêu Đề, Caption & Hashtag TikTok Chuẩn SEO

* **Hook Text trên video (0–3s):** Ngắn dưới 7 từ, đánh vào nỗi đau:  
  * *Ví dụ:* "Đừng bao giờ để bình nước cạnh laptop nếu..." / "Cái kết khi tin lời thằng bạn cùng phòng..."
* **Caption bài viết:**
  * Khơi gợi thảo luận: Đặt một câu hỏi mở để người xem bình luận tranh cãi về cú twist.
  * *Hashtag đề xuất:* `#learnontiktok #gocsangtao #hoathinh3d #reviewcongnghe #[ten_san_pham]`

---

## 4. Đo Lường & Tối Ưu Hóa (A/B Testing 1 Biến Số)

Sau khi đăng tải, theo dõi dữ liệu TikTok Analytics theo 6 chỉ số:

| Chỉ số | Mục tiêu chuẩn | Hành động tối ưu nếu chỉ số thấp |
| :--- | :---: | :--- |
| **1. 3s Retention Rate** | > 65% | Đổi Hook Text trên thumbnail hoặc cắt cảnh 0–1s mở đầu nhanh hơn. |
| **2. Average Watch Time** | > 60% thời lượng | Cắt tỉa nhịp dựng, tăng tốc độ thoại VO thêm 1.1x - 1.15x. |
| **3. Completion Rate** | > 25% | Đẩy cú twist lên sớm hơn, làm twist bất ngờ và ngắn gọn hơn. |
| **4. Shares / Saves** | Cao | Thêm thông tin mẹo vặt hữu ích hoặc tình huống meme cực hài hước. |
| **5. Product Click Rate (CTR)** | > 3% - 5% | Làm nổi bật hơn cảnh sản phẩm giải quyết vấn đề, thêm sticker trỏ giỏ hàng. |
| **6. Đơn hàng (CVR)** | Tùy ngành | Tối ưu trang đích sản phẩm / Flash sale gắn link TikTok Shop. |

> **Nguyên tắc A/B Testing:** Mỗi lần thử nghiệm chỉ thay đổi đúng **1 yếu tố** (hoặc đổi Hook 3 giây đầu, hoặc đổi cú twist cuối) để xác định chính xác nguyên nhân tăng trưởng.
