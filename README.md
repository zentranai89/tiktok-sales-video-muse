# 📱 TikTok Sales Animation Skill (Muse AI)

Skill chuyên sâu sáng tạo video **TikTok bán hàng dạng hoạt hình AI (15–30s, tỷ lệ 9:16)** trên **Muse AI**: từ khâu phân tích sản phẩm, 5 ý tưởng hook & twist, character & product sheets, storyboard match-cut, mega prompt chuẩn hóa realism đến quy trình dựng tối ưu chuyển đổi thương mại.

---

## 🌟 Tính Năng Nổi Bật

Kế thừa triết lý dựng phim từ pipeline chuẩn của **Muse AI** ([`animated_short_film`](https://github.com/sonlovinbot-team/Muse-animated-short-film.git) - Đặng Hữu Sơn), kết hợp với kỹ thuật Marketing giữ chân & chuyển đổi cao của TikTok:

1. **Khóa Tỷ Lệ 9:16 Dọc (STRICT ASPECT RATIO LOCK):** Đảm bảo bố cục điện thoại di động hoàn hảo, không bị biến dạng hình thể khi render.
2. **Khóa Kép Nhân Vật & Sản Phẩm (Character & Product Consistency):** Nhân vật luôn on-model và bao bì/nhãn hiệu sản phẩm giữ nguyên hình dáng, màu sắc qua từng cảnh.
3. **Quy Chuẩn 2–3 Cảnh (15–30s):** Phù hợp với năng lực sinh video ~10s/shot của Muse AI, tối ưu chi phí và thời gian render.
4. **Luật Realism Cơ Học:** Mô tả hành động tương tác với sản phẩm bằng các động tác vật lý thực tế, loại bỏ hoàn toàn các lỗi dị tật AI hay hiệu ứng ảo phi lý.
5. **Kỹ Thuật Match-Cut Liền Mạch:** Nối cảnh tự nhiên giữa Hook và giải pháp sản phẩm, video xem liền mạch như phim chiếu rạp.

---

## 📂 Cấu Trúc Thư Mục Skill

```text
tiktok_sales_video_muse/
├── SKILL.md                                 # File kích hoạt chính của Skill
├── README.md                                # Hướng dẫn sử dụng & tài liệu tổng quan
└── references/
    ├── 01-product-analysis.md               # Phân tích sản phẩm, pain point, visual benefits
    ├── 02-concept-and-hook.md               # 5 ý tưởng hook 3s & twist, rubric chấm điểm
    ├── 03-character-and-product-sheets.md   # Thiết lập Character & Product Sheet khóa 9:16
    ├── 04-storyboard-and-script.md          # Phân cảnh 2-3 shot, cấu trúc 6 nhịp kịch tính
    ├── 05-mega-prompts.md                   # Mẫu Mega Prompt tiếng Anh chuẩn cho Muse AI
    ├── 06-quality-control.md                # Ma trận kiểm soát chất lượng & sửa lỗi prompt
    └── 07-assembly-and-optimization.md      # Hướng dẫn hậu kỳ CapCut/FFmpeg & A/B testing
```

---

## 🚀 Cách Cài Đặt & Sử Dụng

### 1. Dùng trực tiếp trên Antigravity / Gemini CLI:
Skill đã được đặt tại:
`~/.gemini/config/skills/tiktok_sales_video_muse/`

Bạn chỉ cần nhập yêu cầu kèm thông tin sản phẩm, ví dụ:
> *"Hãy áp dụng skill tiktok_sales_video_muse để lên kịch bản video TikTok 20 giây cho sản phẩm [Tên Sản Phẩm]"*

### 2. Xuất bản lên GitHub:
Bạn có thể copy toàn bộ thư mục này và tạo một Git Repository mới trên GitHub để chia sẻ cho cộng đồng người dùng Muse AI!
