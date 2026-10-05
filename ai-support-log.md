# AI Support Log

## Thông tin

- Công cụ AI: GitHub Copilot trong VS Code.
- Ngày làm việc: 2026-10-05.
- Phạm vi ghi log: các yêu cầu và thay đổi được thực hiện trong phiên làm việc này.
- Người nộp bài: Dương Hải Minh - 2A202602680.

## AI đã hỗ trợ

- Đọc `CP3.pdf` và xác định hướng Option A: AI chỉ giải thích ngữ cảnh khi người học chủ động yêu cầu.
- Tạo và chỉnh sửa `Prototype/OptionA.html`: giao diện micro-prototype, nội dung bài giảng về trí nhớ/ngữ cảnh, mục lục kiểu course reader, thao tác chọn highlight, tô/gỡ highlight, tiến độ bài và panel giải thích.
- Tạo các câu trả lời mẫu hard-code cho từng highlight, gồm trường hợp thiếu ngữ cảnh và trường hợp AI không thể giải thích.
- Tạo `three-option-design-sheet.md`, điền Option A theo ảnh được cung cấp và để trống Option B/C theo yêu cầu lúc tạo file.
- Tạo file log này từ lịch sử của phiên làm việc.

## Yêu cầu và quyết định của người nộp bài

- Chọn bài toán “AI Notes: Personal Learning Notes” và yêu cầu xây dựng micro-prototype dựa trên CP3 cùng ảnh đề bài.
- Yêu cầu thêm các đoạn highlight có thể chọn, chuyển giao diện sang bố cục course reader theo ảnh tham chiếu, đưa nút giải thích cạnh highlight, và thêm một highlight đỏ mà AI phải từ chối giải thích bằng câu “Tôi không thể giải thích đoạn này!”.
- Yêu cầu tạo design sheet ba option, trong đó chỉ Option A được điền.

## Kiểm tra đã thực hiện

- Dùng trình duyệt tự động để kiểm tra chọn highlight, mở/đóng panel giải thích, bằng chứng, cảnh báo thiếu ngữ cảnh, tô và gỡ highlight, mục lục, tiến độ, cỡ chữ và điều hướng.
- Xác nhận highlight đỏ trả về đúng câu được yêu cầu; khi chọn lại highlight bình thường, phần bằng chứng được hiển thị lại.
- Kiểm tra tràn ngang ở giao diện desktop và dùng chẩn đoán VS Code cho `Prototype/OptionA.html`; không có lỗi được báo cáo.
- Đây là kiểm tra giao diện tự động, không phải thử nghiệm với người dùng thật.

## Giới hạn cần công khai

- Prototype không kết nối model hoặc API AI. Các giải thích hiển thị là nội dung mẫu được viết sẵn trong mã.
- Bài giảng dài trong `Prototype/OptionA.html` do Copilot soạn cho prototype; nội dung này không được trích nguyên văn từ `CP3.pdf` và chưa được kiểm chứng bằng nguồn học thuật trong phiên này.
- Highlight do người dùng tạo chỉ tồn tại trong trang hiện tại; chưa có lưu trữ backend hoặc đồng bộ sau khi tải lại.
- Nội dung trong file này được tổng hợp từ lịch sử tương tác với Copilot. Người nộp bài cần rà soát, bổ sung hoạt động đã tự làm ngoài phiên này và chỉnh mọi chi tiết chưa phản ánh đúng trải nghiệm thực tế trước khi nộp.