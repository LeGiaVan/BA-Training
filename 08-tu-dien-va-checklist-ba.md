# 08. Từ điển và checklist cho BA

## Từ thường gặp

| Từ | Giải thích ngắn |
| --- | --- |
| BA | Người làm rõ nhu cầu, quy tắc, dữ liệu và tiêu chí nghiệm thu. |
| FAQ | Bộ câu hỏi và trả lời thường gặp. |
| RAG | Cách tìm nội dung liên quan trong tài liệu trước khi tạo câu trả lời. |
| LLM | Công cụ diễn đạt câu trả lời bằng ngôn ngữ tự nhiên. |
| Nguồn trích dẫn | Tài liệu hoặc đoạn nội dung làm căn cứ cho câu trả lời. |
| Hội thoại | Chuỗi câu hỏi và trả lời liên tiếp của một người dùng. |
| Holland / RIASEC | Bài định hướng sở thích; RIASEC là sáu nhóm được chấm điểm. |
| MBTI | Bài mô tả xu hướng theo bốn cặp E/I, S/N, T/F, J/P. |
| ĐGNL | Điểm bài thi Đánh giá năng lực. |
| THPT | Điểm thi tốt nghiệp trung học phổ thông; trong tài liệu này còn dùng để chỉ trường THPT tùy câu. |
| Học bạ | Điểm học tập được dùng khi quy định yêu cầu. |
| CCQT | Chứng chỉ quốc tế như SAT, ACT, IB, A-Level trong phần quy đổi. |
| DT1–DT4 | Bốn nhóm dữ liệu/công thức tính điểm học lực. |
| KV / UT | Khu vực / diện ưu tiên khi tính điểm xét tuyển. |
| BSKT | Bổ sung kiến thức khi dự tuyển sau đại học. |
| Lead | Yêu cầu đăng ký để đơn vị tuyển sinh liên hệ tư vấn. |
| Expected result | Kết quả mong đợi đã được xác nhận để kiểm thử. |
| SLA | Thời hạn phản hồi hoặc xử lý mà đơn vị nghiệp vụ cam kết. |

## Mẫu viết một yêu cầu nghiệp vụ

1. **Ai dùng?** Người dự tuyển Đại học, Sau đại học, phụ huynh hay nhân viên?
2. **Muốn làm gì?** Hỏi thông tin, làm bài, tính điểm, tra bảng hay đăng ký tư vấn?
3. **Cung cấp gì?** Trường bắt buộc, trường tùy chọn, định dạng và giá trị hợp lệ.
4. **Hệ thống xử lý thế nào?** Quy tắc, thứ tự ưu tiên, nguồn, ngưỡng và công thức.
5. **Trả lại gì?** Thông tin hiển thị, cảnh báo, nguồn và bước tiếp theo cho người dùng.
6. **Ngoại lệ là gì?** Thiếu dữ liệu, mã không nhận diện, văn bản mâu thuẫn, gửi thất bại.
7. **Ai xác nhận?** Đơn vị chịu trách nhiệm về nội dung/quy tắc và năm hiệu lực.

## Checklist trước khi chốt yêu cầu

- [ ] Đã gọi đúng tên chức năng trên giao diện và nhóm người dùng.
- [ ] Đã ghi năm tuyển sinh, bậc học và điều kiện áp dụng.
- [ ] Đã có nguồn chính thức và người xác nhận nội dung.
- [ ] Đã phân biệt **trả lời từ tài liệu** với **kết quả tính/tra bảng**.
- [ ] Đã có ví dụ bình thường, thiếu dữ liệu, sai định dạng và trường hợp ranh giới.
- [ ] Đã nói rõ kết quả nào chỉ mang tính tham khảo.
- [ ] Đã xác định dữ liệu cá nhân nào được thu thập và ai xử lý bước tiếp theo.
- [ ] Expected result đủ cụ thể để một người khác kiểm thử mà không phải đoán.

## Bộ test case khởi đầu

| Mã | Thao tác | Điều cần xác nhận |
| --- | --- | --- |
| TC01 | Mở khu vực tư vấn ở phiên mới | Hiện khảo sát nhanh; chỉ tiếp tục khi hồ sơ được tiếp nhận thành công. |
| TC02 | Hỏi học phí của một bậc và năm cụ thể | Câu trả lời đúng bậc/năm, có căn cứ phù hợp nếu hiển thị nguồn. |
| TC03 | Hỏi tiếp “ngành đó thì sao?” | Hiểu đúng ngành vừa hỏi hoặc yêu cầu làm rõ nếu mơ hồ. |
| TC04 | Làm Holland nhưng bỏ trống một mục | Chưa chấm; yêu cầu trả lời đủ. |
| TC05 | Hoàn tất MBTI | Có mã bốn chữ và giải thích đúng theo đáp án đã chọn. |
| TC06 | Tính DT1 khi bỏ trống một điểm THPT | Có cảnh báo; phần trống được tạm dùng như 0 theo luồng hiện tại. |
| TC07 | Tính điểm có điểm cộng vượt trần | Kết quả áp trần điểm cộng và thể hiện cảnh báo. |
| TC08 | Tra BSKT với mã ngành không nhận diện | Chưa hiện kết luận; yêu cầu chọn ngành hoặc nhập lại mã. |
| TC09 | Tra BSKT với ngành hợp lệ | Hiện bảng nhiều ngành dự tuyển, ba trạng thái và môn cần học khi có. |
| TC10 | Gửi đăng ký tư vấn với một trường bắt buộc trống | Không gửi; chỉ ra phần cần bổ sung. |
| TC11 | Gửi đăng ký khi một kênh tiếp nhận thành công | Báo đã tiếp nhận; nếu kênh thông báo lỗi, thể hiện cảnh báo phù hợp. |
| TC12 | Thay thông báo tuyển sinh cũ bằng văn bản mới | Câu trả lời theo văn bản có hiệu lực; không trộn mốc cũ và mới. |
| TC13 | FAQ và tài liệu cùng nói về một vấn đề nhưng ghi kết quả khác nhau | Xác nhận văn bản có hiệu lực với đơn vị nghiệp vụ; kết quả trả lời và nguồn phải theo quyết định đã chốt. |

## Năm câu hỏi BA nên mang đến buổi làm rõ

1. Văn bản nào là nguồn chuẩn nếu FAQ và thông báo mới khác nhau?
2. Quy tắc áp dụng cho năm, bậc, đợt và phương thức xét tuyển nào?
3. Ai duyệt công thức, bảng quy đổi, danh mục BSKT và nội dung trả lời?
4. Sau khi nhận lead, ai phụ trách liên hệ và trong thời gian bao lâu?
5. Với dữ liệu cá nhân và lịch sử tư vấn, ai được xem và giữ trong bao lâu?
