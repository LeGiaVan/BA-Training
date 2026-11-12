# Cẩm nang nghiệp vụ Chatbot tư vấn tuyển sinh UEL

Tài liệu này dành cho **BA thực tập** mới tham gia dự án. Chỉ cần đọc thư mục này là có thể hiểu các chức năng người dùng nhìn thấy, quy trình xử lý chính và những câu hỏi cần làm rõ với đơn vị nghiệp vụ. Tài liệu dùng từ đơn giản; các tên chuyên ngành như Holland, MBTI, RAG, ĐGNL được giữ nguyên.

## Lộ trình đọc

| Thứ tự | Tài liệu | Trả lời câu hỏi |
| --- | --- | --- |
| 1 | [Tổng quan dự án](01-tong-quan.md) | Dự án phục vụ ai, giải quyết nhu cầu gì? |
| 2 | [Bản đồ chức năng](02-ban-do-chuc-nang.md) | Người dùng có thể làm những gì? |
| 3 | [Quy trình hỏi đáp tuyển sinh](03-hoi-dap-tuyen-sinh.md) | Một câu hỏi được xử lý và trả lời ra sao? |
| 4 | [Trắc nghiệm và tính điểm](04-trac-nghiem-va-tinh-diem.md) | Holland, MBTI và điểm xét tuyển được xử lý thế nào? |
| 5 | [Bổ sung kiến thức](05-bo-sung-kien-thuc.md) | Khi nào được miễn hoặc phải học bổ sung? |
| 6 | [Khảo sát và đăng ký tư vấn](06-khao-sat-dang-ky-va-du-lieu.md) | Hệ thống thu thập, tiếp nhận thông tin gì? |
| 7 | [Quản lý nội dung tư vấn](07-nguon-tri-thuc-va-cap-nhat.md) | Thông tin trả lời đến từ đâu và cập nhật thế nào? |
| 8 | [Từ điển và checklist BA](08-tu-dien-va-checklist-ba.md) | Viết yêu cầu và kiểm thử từ đâu? |
| 9 | [Cơ chế chọn chunk Qdrant](09-co-che-chon-chunk-qdrant.md) | Khi nhiều tài liệu được tìm thấy, hệ thống chọn đoạn nào để trả lời? |

## Cách dùng tài liệu

- Đọc **quy trình chính** trước, sau đó xem **ngoại lệ** và **quy tắc nghiệp vụ**. Khi viết yêu cầu, luôn ghi rõ chức năng, nhóm người dùng, năm tuyển sinh và nguồn thông tin có hiệu lực.
- Các sơ đồ dùng Mermaid. Nếu GitHub không hiển thị sơ đồ, phần diễn giải ngay bên dưới vẫn mô tả đủ các bước.
- Các ví dụ về điểm và lịch chỉ giúp hiểu cách xử lý. **Thông báo tuyển sinh và quyết định của UEL** mới là căn cứ cuối cùng cho từng kỳ tuyển sinh.

## Điều cần nhớ

Hệ thống có hai loại kết quả: **tra cứu/tư vấn** từ tài liệu và **tính/đối chiếu** từ quy tắc, bảng dữ liệu. Kết quả trắc nghiệm và tính điểm có tính tham khảo. Việc đăng ký tư vấn là bước gửi yêu cầu cho nhà trường; quy trình nhân viên liên hệ sau đó cần được đơn vị phụ trách xác nhận riêng.
