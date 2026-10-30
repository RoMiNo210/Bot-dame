WEBSITE CHECKER — HTML + PYTHON

Mục đích:
- Kiểm tra website còn phản hồi không.
- Đo thời gian phản hồi và xem mã HTTP (bản Python).
- Tự động kiểm tra theo chu kỳ, có số lần giới hạn.

HTML:
1. Mở index.html trong trình duyệt.
2. Nhập URL.
3. Đặt số lần kiểm tra (tối đa 100) và khoảng cách (ít nhất 10 giây).
4. Nhấn Bắt đầu hoặc Dừng.
Lưu ý: Trình duyệt có thể chặn đọc phản hồi từ website khác do CORS. Bản HTML có thể chỉ xác nhận đã gửi yêu cầu, không đọc được mã HTTP.

PYTHON:
Cần Python 3.
Cài thư viện:
    python -m pip install requests

Chạy ví dụ:
    python website_checker.py https://example.com --count 10 --interval 30

Tham số:
    --count       1 đến 100 lần kiểm tra
    --interval    tối thiểu 10 giây giữa các lần

Dừng:
- Nhấn Ctrl+C.

An toàn:
- Chỉ sử dụng trên website bạn sở hữu hoặc có sự cho phép kiểm thử.
- Công cụ cố ý không có xoay IP, proxy rotation, truy cập song song hoặc chế độ tạo lượt xem giả.
- Đừng tăng tốc độ hoặc số yêu cầu để làm gián đoạn dịch vụ.
