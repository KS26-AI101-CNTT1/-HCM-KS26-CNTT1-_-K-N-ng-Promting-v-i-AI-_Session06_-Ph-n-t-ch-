Đề bài / Yêu cầu

So sánh Trade-off các giải pháp ra lệnh cho Ứng dụng AI trong Học tập & Nghiên cứu

1. Mục tiêu bài tập dễ hiểu

Rèn luyện tư duy phản biện. Sinh viên đề xuất 2 giải pháp viết prompt khác nhau cho chủ đề Ứng dụng AI trong Học tập & Nghiên cứu và so sánh xem phương án nào tối ưu nhất.

2. Bối cảnh & yêu cầu bài toán

Bài toán yêu cầu thực hiện tối ưu hóa quy trình Feynman Prompt gia sư, Rubric chấm bài tự động.

3. Quy tắc nghiệp vụ

Đưa ra Giải pháp 1 (đơn giản, ngắn gọn) và Giải pháp 2 (chi tiết, có nhiều ràng buộc).

4. Ràng buộc & bẫy dữ liệu

Lập bảng so sánh tiêu chí để đánh giá ưu nhược điểm rõ ràng.

5. Yêu cầu bài làm chi tiết

Bước 1: Đề xuất 2 prompt mẫu

Viết rõ 2 prompt tương ứng với 2 phương án giải quyết.

1. Giải pháp 1 (Đơn giản, ngắn gọn) [1]

Đóng vai gia sư Feynman và người chấm bài. Dựa vào đề bài: "{{de_bai}}", thang điểm: "{{rubric}}", hãy chấm điểm bài làm: "{{bai_lam}}". Chỉ ra lỗi sai và giải thích lại bằng ngôn ngữ đơn giản nhất kèm ví dụ thực tế.

2. Giải pháp 2 (Chi tiết, nhiều ràng buộc) [1]

 [VAI TRÒ] Hệ thống chấm điểm tự động tích hợp Gia sư Feynman.

[ĐẦU VÀO] Đề: {{de_bai}} | Rubric: {{rubric}} | Bài làm: {{bai_lam}}

[RÀNG BUỘC]

1. Chặn lỗi: Nếu {{bai_lam}} rỗng, vô nghĩa (spam) hoặc lạc đề -> DỪNG CHẤM, yêu cầu nộp lại bài.

2. Khách quan: Chấm đúng khung {{rubric}}, không tự ý thêm bớt điểm.

3. Feynman: Giải thích lỗi sai như dạy trẻ 12 tuổi (cấm thuật ngữ khó), bắt buộc có 1 ví dụ đời thường + 1 câu hỏi gợi mở.

[ĐẦU RA] Phần 1: Bảng điểm chi tiết | Phần 2: Giải thích Feynman.

Bước 2: Lập bảng so sánh Trade-off

Lập bảng so sánh tiêu chí.

Tiêu chí	Giải pháp 1 (Đơn giản)	Giải pháp 2 (Chi tiết)

Độ dễ hiểu	Cao	Trung bình

Tốn token	Ít	Nhiều hơn

Chặn lỗi biên	Trung bình	Cực tốt

Tiêu chí	Giải pháp 1 (Đơn giản)	Giải pháp 2 (Chi tiết)

Độ dễ hiểu	Cao (dễ viết, triển khai nhanh)	Trung bình (cần cấu trúc luật rõ ràng)

Tốn token	Ít (tiết kiệm chi phí)	Nhiều hơn (tốn thêm ~150 token ràng buộc)

Chặn lỗi biên	Trung bình (dễ chấm bừa khi gặp bài rác)	Cực tốt (chặn đứng dữ liệu rác, lạc đề)

Độ ổn định đầu ra	Thấp (bố cục thay đổi ngẫu nhiên)	Rất cao (chuẩn khuôn mẫu, dễ tự động hóa)

Bước 3: Lựa chọn và chạy thử

Chọn phương án tối ưu nhất, giải thích lý do chọn và chạy thử lấy kết quả.

Lựa chọn: Giải pháp 2.

Lý do: Trong giáo dục, độ chính xác và khả năng chặn dữ liệu rác quan trọng hơn việc tiết kiệm một ít token. Giải pháp 2 đảm bảo AI chấm đúng thang điểm và giữ đúng chuẩn sư phạm Feynman.

Kết quả chạy thử Giải pháp 2:

Input: Đề: Cơ chế bộ nhớ đệm (Cache) | Rubric: Bản chất (5đ), Cơ chế (5đ) | Bài làm: "Cache là ổ cứng lưu dữ liệu vĩnh viễn khi tắt máy."

Output của AI:

Phần 1: Bảng điểm

Bản chất (0/5đ): Sai kiến thức, nhầm Cache với ổ cứng.

Cơ chế (0/5đ): Chưa nêu được cơ chế truy xuất.

Tổng: 0/10 điểm.

Phần 2: Giải thích Feynman

Đơn giản: Ổ cứng mới lưu dữ liệu vĩnh viễn, còn Cache là trí nhớ siêu ngắn hạn nằm cạnh CPU, chỉ giữ tạm dữ liệu vừa dùng và sẽ xóa sạch khi tắt máy.

Ví dụ: Ổ cứng là thư viện lớn cuối phố, còn Cache là mặt bàn học trước mặt bạn để đặt sẵn 3 cuốn sách hay dùng nhất cho tiện lấy.

Câu hỏi: Nếu mặt bàn (Cache) đã đầy sách mà bạn muốn lấy thêm sách mới từ thư viện về thì máy sẽ làm gì?
