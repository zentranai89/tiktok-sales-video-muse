---
name: "tiktok_sales_video_muse"
description: "Skill chuyên sâu sáng tạo video TikTok bán hàng hoạt hình ngắn (15–30s, tỷ lệ 9:16) trên Muse AI: phân tích sản phẩm, 5 concept hook/twist, character & product sheets, storyboard match-cut, mega prompt chuẩn hóa realism và quy trình dựng tối ưu chuyển đổi."
---

# TikTok AI Commercial Animation Pipeline (Muse AI)

**Định dạng:** Video dọc 9:16 (720×1280 / 1080×1920) | Thời lượng: 15–30 giây | Nền tảng: Muse AI & TikTok Shop  
**Mục tiêu:** Chuyển hóa tính năng sản phẩm thành video hoạt hình hài hước, giữ chân 0–3 giây đầu, có cú twist bất ngờ và tích hợp sản phẩm tự nhiên để kích hoạt chuyển đổi.

---

## 🎯 Cốt lõi kỹ thuật trên Muse AI

Skill này kết hợp **chiến lược Marketing TikTok chuyển đổi cao** với **Pipeline hoạt hình chuẩn mực của Muse AI** (kế thừa triết lý từ dự án *The Last Lantern* của Đặng Hữu Sơn):
1. **Khóa tỷ lệ dọc tuyệt đối (STRICT ASPECT RATIO LOCK 9:16):** Mọi reference (nhân vật, sản phẩm, keyframe) phải chuẩn 9:16 dọc để không vỡ khung hình.
2. **Khóa kép Nhân vật & Sản phẩm:** Giữ nhân vật on-model và bao bì/hình dáng sản phẩm đồng nhất 100% qua các shot.
3. **Quy tắc số cảnh chuẩn Muse AI (10s/shot):** Video 15–20s = đúng **2 cảnh**; video 25–30s = đúng **3 cảnh**. Không chia cảnh vụn.
4. **Luật Realism cơ học:** Tương tác với sản phẩm phải đúng vật lý (mở nắp, xịt, bấm nút, bôi thoa). Không dùng động từ trừu tượng.
5. **Match-Cut tự nhiên:** Frame cuối cảnh N nối liền với frame đầu cảnh N+1.

---

## 🚦 Giai đoạn 0 — Thu thập đầu vào (BẮT BUỘC)

Trước khi viết kịch bản, cần xác định 4 thông số:
1. **Sản phẩm & USP (Điểm bán hàng độc nhất):** Tên sản phẩm, công dụng then chốt có thể thấy bằng mắt, đối tượng khách hàng mục tiêu.
2. **Thời lượng mong muốn (Số cảnh):**
   * **15–20 giây:** 2 cảnh (Cảnh 1: Hook + Pain Point; Cảnh 2: Product + Twist). Cắt gọt lúc dựng.
   * **25–30 giây:** 3 cảnh (Cảnh 1: Hook 8s; Cảnh 2: Escalation & Product 10s; Cảnh 3: Twist & Payoff 8-10s).
3. **Phong cách thị giác (Visual Style):** 3D Stylized (Pixar/Illumination style commercial) hoặc 2D Anime/Chibi tươi sáng.
4. **Ngôn ngữ kịch bản & VO:** Tiếng Việt / Tiếng Anh.

---

## 🔄 Workflow 8 Bước Sản Xuất

Làm theo đúng thứ tự 8 bước. Mỗi bước có tài liệu hướng dẫn và checklist chi tiết trong `references/`:

1. **Phân tích sản phẩm thương mại** → `references/01-product-analysis.md`
   * Bóc tách Pain Point, Visual Benefit, tình huống trớ trêu đời thường, ranh giới pháp lý/claim.
2. **5 Ý tưởng Hook & Twist** → `references/02-concept-and-hook.md`
   * Lên 5 concept có hook 3s đầu, bảng chấm điểm 5 tiêu chí: Hook, Hài hước, Giữ chân, Tích hợp sản phẩm, Tiềm năng chuyển đổi. Chốt 1 ý tưởng xuất sắc nhất.
3. **Character & Product Reference Sheets** → `references/03-character-and-product-sheets.md`
   * Thiết lập mô tả chuẩn cho Character Sheet (khóa nhân vật) và Product Sheet (khóa bao bì, logo, kích thước tỷ lệ). Tỷ lệ 9:16 dọc.
4. **Storyboard & Match-Cut Continuity** → `references/04-storyboard-and-script.md`
   * Cấu trúc kịch bản: `HOOK → SETUP → ESCALATION → PRODUCT INTEGRATION → TWIST → ENDING`. Khóa keyframe giao thoa giữa các cảnh.
5. **Bộ Mega Prompts Muse AI** → `references/05-mega-prompts.md`
   * Viết prompt tiếng Anh chuẩn "copy-paste là chạy" cho từng cảnh: Global Locks, Character Lock, Product Lock, First Frame, Motion Realism, Camera, Last Frame, Sound, Music, VO.
6. **Kiểm soát chất lượng (QC)** → `references/06-quality-control.md`
   * Kiểm tra dị tật tay chân, méo bao bì sản phẩm, chuyển động phi logic, nhịp dựng. Sửa prompt thay vì chấp nhận clip lỗi.
7. **Hậu kỳ & Hoàn thiện** → `references/07-assembly-and-optimization.md`
   * Quy chuẩn dựng CapCut / FFmpeg (720×1280, 24/30fps), ducking âm thanh, phụ đề động, caption & hashtag bắt trend.
8. **Đo lường & Tối ưu chuyển đổi (A/B Test)** → `references/07-assembly-and-optimization.md`
   * Đo lường 6 chỉ số: Watch Time, Completion Rate, Profile Visits, CTR giỏ hàng, CVR. Kỹ thuật test 1 biến số.

---

## 📋 Output Contract

Khi hoàn thành dự án, bạn sẽ có trọn bộ tư liệu:
- `PRODUCT_BRIEF.md`: Bản phân tích tính năng và 5 ý tưởng chấm điểm.
- `STORY_AND_SCRIPT.md`: Kịch bản chi tiết theo từng giây và bảng Storyboard.
- `REFERENCE_PROMPTS.md`: Prompt vẽ Character Sheet và Product Sheet chuẩn 9:16.
- `MEGA_PROMPTS.md`: Bộ prompt Muse AI độc lập cho từng cảnh.
- `ASSEMBLY_GUIDE.md`: Hướng dẫn dựng video, text hook, nhạc nền, caption và checklist nghiệm thu.

---

## ⚠️ Nguyên Tắc Bắt Buộc (Operating Rules)

1. **Khóa 9:16 Vertical:** Toàn bộ ảnh ref, keyframe và prompt sinh video đều phải tuân thủ nghiêm ngặt khung dọc 9:16.
2. **Thứ tự nạp Reference vào Muse AI:**
   * 1: `CHARACTER_SHEET`
   * 2: `PRODUCT_SHEET`
   * 3: `FIRST_FRAME_KEYFRAME`
   * 4: `LAST_FRAME_KEYFRAME`
3. **Luật Realism khi tương tác với sản phẩm:** Mọi động tác cầm nắm, mở nắp, bấm nút, thoa/xịt/uống phải miêu tả cơ chế vật lý thật. Không bao giờ viết "dùng sản phẩm và phép màu xảy ra".
4. **Sản phẩm là mắt xích giải quyết mâu thuẫn:** Sản phẩm không phải phụ kiện nền, cũng không được phóng đại sai sự thật.
5. **Cú twist phục vụ ghi nhớ, không gây hiểu lầm:** Twist mang lại tiếng cười sảng khoái và làm nổi bật tính năng thật của sản phẩm.
