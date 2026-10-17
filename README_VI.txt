VHUU VIP WEB CLIP KIT

Trong gói này có:
- site/index.html: giao diện web có avatar, ô nhập key và dashboard công tắc.
- site/assets/avatar.png: avatar.
- profile/generate_profile.py: tạo file .mobileconfig sau khi website đã được đưa lên hosting HTTPS.

CÁCH DÙNG
1. Đưa toàn bộ nội dung thư mục site lên một dịch vụ hosting static có HTTPS (ví dụ GitHub Pages, Netlify hoặc Cloudflare Pages).
2. Mở URL HTTPS của website để kiểm tra giao diện.
3. Trên máy có Python 3, chạy:
   cd profile
   python3 generate_profile.py https://TEN-MIEN-CUA-BAN/
4. File VhuuVip_WebClip.mobileconfig được tạo trong thư mục profile. Gửi file đó sang iPhone, mở file và làm theo hướng dẫn cài cấu hình.
5. Nếu muốn cập nhật website, tải bản site mới lên hosting; Web Clip sẽ mở cùng địa chỉ đó.

LƯU Ý
- Chưa thể tạo file .mobileconfig hoàn chỉnh có URL thật cho đến khi có địa chỉ HTTPS hosting của bạn.
- Key VhuuVip hiện được kiểm tra trong JavaScript phía trình duyệt. Đây chỉ là khóa giao diện, không phải bảo mật thật; người biết cách xem mã nguồn có thể tìm thấy key. Muốn bảo vệ thực sự cần xác thực phía máy chủ.
- Các công tắc chỉ là trạng thái giao diện, không điều khiển iOS hay game.
- Web Clip không phải ứng dụng native và cần internet để tải website lần đầu/mỗi lần mở nội dung chưa lưu.
