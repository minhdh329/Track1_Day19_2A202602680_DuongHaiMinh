# AI Notes: Personal Learning Notes

Micro-prototype cho người học muốn khôi phục ngữ cảnh của một đoạn đã highlight khi ôn tập. Người học chủ động chọn đoạn và gọi AI; prototype Option A hiện là giao diện tĩnh với câu trả lời mẫu.

**Prototype Option A:** [Mở GitHub Pages](https://minhdh329.github.io/Track1_Day19_2A202602680_DuongHaiMinh/)

## 1. Thông tin cá nhân và đội ngũ

- Họ tên: Dương Hải Minh
- Mã sinh viên: 2A202602680
- Case bài toán: AI Notes — Personal Learning Notes

| Thành viên | Họ tên | Mã sinh viên | Vai trò trong nhóm |
| --- | --- | --- | --- |
| 1 | Dương Hải Minh | 2A202602680 | Prototype Option A |
| 2 | Tô Anh Đức | 2A202602639 | Prototype Option C |
| 3 | Đỗ Trương Thành Ân | 2A202602899 | Prototype Option B |

## 2. Hypothesis Problem

**Hypothesis chính thức của nhóm tại Day 18:** 
**Khi người dùng take note hoặc highlight bài giảng, rồi sử dụng AI ở ngoài trả lời, thì câu trả lời của AI thường bị out of context (thiếu ngữ cảnh), rời rạc, lạc đề khỏi bài giảng.**

Bản nháp để đối chiếu với câu Day 18, không thay thế hypothesis chính thức:

> Khi người học ôn lại ghi chú cá nhân và gặp một highlight đã quên lý do hoặc ngữ cảnh, họ cần cách hiểu nhanh đoạn xung quanh vì tự lần lại tài liệu gây gián đoạn; AI chỉ nên giải thích khi được gọi để tránh làm nhiễu nội dung học.

Các thành tố cần xác nhận theo framework 5 phần nhóm dùng ở Day 18:

| Thành tố | Nội dung đã biết / cần nhóm xác nhận |
| --- | --- |
| Người dùng | Người học ghi chú cá nhân. Persona cụ thể chưa được xác nhận trong tài liệu hiện có. |
| Bối cảnh | Đang ôn tập và gặp lại highlight không còn nhớ ngữ cảnh |
| Nhu cầu/vấn đề | Khôi phục nhanh ý nghĩa của đoạn được highlight |
| Rào cản | Phải tự đọc lại phần văn bản xung quanh; có thể làm gián đoạn việc ôn |
| Insight/giả định | Người học chỉ quên một số highlight; AI nên chờ yêu cầu thay vì tự động giải thích tất cả |

## 3. Three Solution Options

| Option | Cơ chế hoạt động | Trạng thái prototype/link |
| --- | --- | --- |
| **A — User Initiates / Truy xuất theo yêu cầu** | Khi ôn tập, người học chọn highlight chưa hiểu và yêu cầu AI tóm tắt ngữ cảnh từ đoạn trước/sau. AI trả lời ngắn trong panel; có căn cứ, giới hạn và cách đóng để quay lại ghi chú. | [Trải nghiệm Option A](https://minhdh329.github.io/Track1_Day19_2A202602680_DuongHaiMinh/). Prototype hiện dùng nội dung mẫu, không gọi model/API thật. |
| **B — Conditional Checkpoint & Batch Synthesis** | AI theo dõi highlight và bullet take-note; khi tổng số đạt 5, hỏi người học có muốn tổng hợp ngay không. Nếu hoãn, AI tổng hợp khi kết thúc phiên. | [Trải nghiệm Option B](https://track1day192a202602899dotruongthanhan-production.up.railway.app/). Cơ chế theo design sheet; cần đối chiếu hành vi thực tế của prototype với mô tả này. |
| **C — Proactive Context & Constrained Chat** | Khi người học lưu highlight, AI tự viết 2-3 câu giải thích ngữ cảnh. Chat chỉ dựa trên note đã lưu và ngữ cảnh AI tạo; từ chối câu hỏi ngoài phạm vi. | [Trải nghiệm Option C](https://ainote-itt9q3xqj-anhduc0712s-projects.vercel.app/). Cơ chế theo design sheet; cần đối chiếu hành vi thực tế của prototype với mô tả này. |

Design sheet: [three-option-design-sheet.md](three-option-design-sheet.md). Link tổng hợp: [prototype-link.md](prototype-link.md).

## 4. Đóng góp cụ thể của tôi trong sản phẩm nhóm

**Bản tự thuật theo phạm vi phiên làm việc này; người nộp bài cần chỉnh nếu khác đóng góp thực tế trong nhóm:**

- Phụ trách phát triển prototype Option A theo hướng user-initiated/context on-demand.
- Xác định và tinh chỉnh luồng chọn highlight, gọi giải thích, xem câu làm căn cứ, đóng panel và quay lại ghi chú.
- Đề xuất các trạng thái đủ/thiếu ngữ cảnh và một highlight đỏ để thể hiện trường hợp AI không thể giải thích.
- Dùng GitHub Copilot để tạo/chỉnh sửa HTML và nội dung prototype; phản hồi yêu cầu và kiểm tra lại tương tác bằng trình duyệt.
- Tài liệu hiện có không phân định cụ thể phần đóng góp cá nhân vào bối cảnh chung, Human–AI Decision Table và các option B/C; người nộp bài cần bổ sung nếu có tham gia.

## 5. Dữ liệu kiểm thử và bài học

**Tình trạng hiện tại:** workspace có ba feedback note cho các phiên ngày 05/10/2026. Đây là ghi chép định tính với ba tester, không có số đo thời gian hay thước đo hiệu quả học tập. Chi tiết nằm trong [prototype-feedback-note.md](prototype-feedback-note.md); phần đối chiếu nằm trong [group-feedback-synthesis.md](group-feedback-synthesis.md).

### Tổng hợp ba phiên của nhóm

| Phiên | Người thử / option | Quan sát và phản hồi thực tế | Kết quả / bài học |
| --- | --- | --- | --- |
| 1 | Tester 1 — chọn B | Tìm định nghĩa để highlight; không ghi nhận do dự; dùng nút tắt trên câu trả lời AI. Sẵn sàng take note lâu hơn để nhận giải thích cô đọng. Ô kiểm tra nguồn trong phiếu để trống. | Ưu tiên nội dung cô đọng dù tốn thao tác; không có ghi nhận về việc kiểm tra nguồn. |
| 2 | Tester 2 — chọn C | Bắt đầu bằng chuyển slide; hiểu nhầm rằng phải bấm nút mới mở note; có kiểm tra nguồn/cảnh báo; tạo chat mới để làm lại. Thích giải thích ngay của C và tổng hợp của B. | Cần làm rõ cách mở note; phản hồi gợi ý kiểm thử kết hợp giải thích tại highlight với tổng hợp của B. |
| 3 | Tester 3 — chọn A | Cố highlight đoạn cần note; không ghi nhận do dự; kiểm tra lại nguồn; dùng nút tắt trên AI. Ưu tiên tiện lợi hơn độ chi tiết. | Ưu tiên tiện lợi, đối lập với lựa chọn chấp nhận thêm thời gian để có giải thích cô đọng ở Phiên 1. |

### Next Change

- Quyết định sau tổng hợp ba phiên: kiểm thử một luồng ghi chú kết hợp, trong đó người học chủ động gọi giải thích ngữ cảnh ngay tại highlight và xem các giải thích đã gom trong bản tổng hợp cuối phiên; không tự bật lời nhắc giữa giờ. Đây là thay đổi cần kiểm thử, chưa phải kết luận triển khai.
- Cơ sở: mỗi option A, B, C được chọn một lần; Tester 2 thích giải thích tức thì của C và khả năng tổng hợp của B; Tester 1 chấp nhận thêm thời gian để có giải thích cô đọng, còn Tester 3 ưu tiên tiện lợi.

### Still Unproven

- Người chưa từng xem prototype có tự phát hiện và chọn đúng highlight cần giải thích không.
- Giải thích, câu làm căn cứ và thông báo giới hạn có giúp người học đánh giá độ tin cậy không.
- Người học có thấy việc gọi AI từng đoạn là đủ hữu ích so với công sức thao tác không.
- Trạng thái “không đủ thông tin” và câu trả lời từ chối có được hiểu đúng không.
- Luồng kết hợp đề xuất có dễ dùng và ít gián đoạn hơn không; tổng hợp cuối phiên có giúp nhớ lại bài hoặc tiết kiệm thời gian không. Ba phiên hiện tại chưa đo các kết quả này, và chưa đủ cơ sở kết luận option nào được ưa thích hơn.

## 6. AI Support Log

- Công cụ đã dùng: GitHub Copilot trong VS Code. Log chi tiết: [ai-support-log.md](ai-support-log.md).
- Copilot hỗ trợ đọc `CP3.pdf`, tạo/chỉnh sửa `Prototype/OptionA.html`, nội dung bài giảng mẫu, tương tác highlight, panel giải thích, bố cục course reader, design sheet và các mẫu tài liệu.
- Người nộp bài cung cấp mục tiêu, ảnh tham chiếu và yêu cầu sửa qua các vòng; cần rà soát nội dung và bổ sung các đóng góp thực tế ngoài phiên này.
- Prototype không gọi AI model/API thật: các phản hồi giải thích được viết sẵn. Nội dung bài giảng do AI soạn, không trích nguyên văn CP3 và chưa được kiểm chứng bằng nguồn học thuật trong phiên này.
- Kiểm tra trình duyệt tự động chỉ xác nhận tương tác giao diện; không thay thế ba phiên thử nghiệm với người dùng. Ba feedback note hiện có là ghi chép từ các phiên test, nhưng số lượng nhỏ và chưa có thước đo định lượng.