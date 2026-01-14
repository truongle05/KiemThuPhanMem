# KiemThuPhanMem
Bài tập thực hành tuần 1 – Trải nghiệm và đánh giá chất lượng giao diện phần mềm
1. Mục tiêu bài thực hành

Bài thực hành tuần 1 nhằm giúp sinh viên:

Làm quen với việc học cá nhân hoá thông qua công cụ NotebookLM

Trải nghiệm và đánh giá chất lượng giao diện người dùng (UI) của phần mềm

Rèn luyện khả năng quan sát, phát hiện lỗi giao diện

Bước đầu hình thành tư duy kiểm thử giao diện trong kiểm thử phần mềm

Tạo và quản lý báo cáo thực hành trên GitHub Repository

2. Quá trình thực hiện
2.1. Học tập với NotebookLM

Sinh viên truy cập vào công cụ NotebookLM theo đường dẫn được cung cấp để:

Xem video và nghe audio liên quan đến nội dung học

Đặt câu hỏi và trao đổi với NotebookLM nhằm hiểu rõ hơn về các khái niệm

Học tập theo hình thức cá nhân hoá, chủ động tiếp cận kiến thức

Công cụ NotebookLM hỗ trợ sinh viên tiếp thu kiến thức linh hoạt, giúp làm quen với việc ứng dụng mô hình ngôn ngữ lớn (LLM) trong học tập.

2.2. Trải nghiệm chất lượng giao diện với Can’t Unsee

Sau khi học tập với NotebookLM, sinh viên thực hiện bài trải nghiệm giao diện tại trang web:
👉 https://cantunsee.space/

Quá trình làm bài diễn ra như sau:

Sinh viên truy cập trang web và bắt đầu trò chơi Can’t Unsee

Mỗi màn chơi yêu cầu so sánh hai giao diện gần giống nhau

Nhiệm vụ là phát hiện các lỗi nhỏ trong thiết kế giao diện như:

Căn chỉnh sai

Khoảng cách không đều

Bố cục thiếu nhất quán

Các chi tiết UI gây ảnh hưởng đến trải nghiệm người dùng

Sinh viên lựa chọn vị trí giao diện bị lỗi theo yêu cầu hệ thống

Trong quá trình thực hiện, các lỗi có độ khó tăng dần, đòi hỏi sinh viên phải quan sát kỹ, tập trung và vận dụng tư duy đánh giá giao diện.

3. Kết quả đạt được

Sau khi hoàn thành bài trải nghiệm, hệ thống ghi nhận kết quả như sau:

Điểm số: 6030 điểm

Xếp hạng: Beginner

Thời gian hoàn thành: 00:06:02

Sinh viên đã chụp ảnh màn hình kết quả, trong đó có dấu hiệu cá nhân (đăng nhập trình duyệt Chrome), và đưa hình ảnh này lên GitHub Repository theo đúng yêu cầu bài tập.

4. Nhận xét và đánh giá

Thông qua bài thực hành này, sinh viên nhận thấy:

Việc phát hiện lỗi giao diện nhỏ là khó khăn nhưng rất quan trọng

Những sai lệch nhỏ trong UI có thể ảnh hưởng lớn đến trải nghiệm người dùng

Trò chơi Can’t Unsee giúp rèn luyện tư duy kiểm thử giao diện một cách trực quan

Đây là nền tảng cần thiết để tiếp cận các công cụ kiểm thử giao diện chuyên sâu như Cypress hoặc Playwright trong các tuần tiếp theo

5. Kết luận

Bài thực hành tuần 1 giúp sinh viên làm quen với phương pháp học tập hiện đại thông qua NotebookLM và bước đầu tiếp cận hoạt động đánh giá chất lượng giao diện phần mềm. Việc trải nghiệm Can’t Unsee mang lại cái nhìn thực tế về tầm quan trọng của UI/UX trong kiểm thử phần mềm và tạo tiền đề cho các bài thực hành nâng cao sau này.




Bài thực hành kiểm thử tự động End-to-End với Cypress
1. Mục tiêu bài thực hành

Mục tiêu của bài thực hành là giúp sinh viên làm quen và thực hành kiểm thử tự động End-to-End (E2E) bằng công cụ Cypress. Thông qua việc xây dựng các kịch bản kiểm thử trên một trang web mẫu, sinh viên hiểu được quy trình kiểm thử giao diện người dùng, kiểm thử chức năng và xác minh hành vi của hệ thống một cách tự động.

2. Công cụ và môi trường sử dụng

Ngôn ngữ: JavaScript

Công cụ kiểm thử: Cypress

Phiên bản Cypress: 15.9.0

Môi trường phát triển: Visual Studio Code

Nền tảng chạy kiểm thử: Google Chrome

Website kiểm thử: https://www.saucedemo.com

Hệ điều hành: Windows

3. Cài đặt và cấu hình Cypress

Quá trình cài đặt Cypress được thực hiện theo các bước sau:

Tạo thư mục dự án và khởi tạo npm.

Cài đặt Cypress bằng npm.

Mở Cypress UI bằng lệnh npx cypress open.

Chọn chế độ E2E Testing và trình duyệt Chrome.

Tạo thư mục cypress/e2e và các file kiểm thử theo chuẩn .cy.js.

Cypress UI được sử dụng để chạy và theo dõi kết quả kiểm thử, trong khi mã nguồn kiểm thử được viết bằng Visual Studio Code.

4. Các kịch bản kiểm thử đã thực hiện
4.1. Kiểm thử đăng nhập thành công

Nhập tài khoản hợp lệ: standard_user / secret_sauce

Nhấn nút Login

Xác minh người dùng được chuyển đến trang danh sách sản phẩm (/inventory.html)

Kết quả: Test chạy thành công, hệ thống hoạt động đúng như mong đợi.

4.2. Kiểm thử đăng nhập thất bại

Nhập thông tin đăng nhập không hợp lệ

Nhấn Login

Kiểm tra thông báo lỗi hiển thị

Kết quả: Thông báo lỗi được hiển thị đúng, test PASS.

4.3. Kiểm thử thêm sản phẩm vào giỏ hàng

Đăng nhập thành công

Thêm một sản phẩm vào giỏ hàng

Kiểm tra số lượng sản phẩm trong biểu tượng giỏ hàng

Kết quả: Sản phẩm được thêm thành công, số lượng hiển thị chính xác.

4.4. Kiểm thử sắp xếp sản phẩm theo giá

Chọn bộ lọc “Price (low to high)”

Kiểm tra giá sản phẩm đầu tiên trong danh sách

Kết quả: Sản phẩm được sắp xếp đúng theo giá tăng dần.

4.5. Kiểm thử xóa sản phẩm khỏi giỏ hàng

Thêm sản phẩm vào giỏ hàng

Nhấn nút “Remove”

Kiểm tra biểu tượng giỏ hàng không còn hiển thị số lượng

Kết quả: Sản phẩm được xóa thành công khỏi giỏ hàng.

4.6. Kiểm thử quy trình thanh toán

Đăng nhập và thêm sản phẩm vào giỏ hàng

Truy cập trang thanh toán

Nhập thông tin người dùng (First Name, Last Name, Zip Code)

Nhấn Continue và kiểm tra URL

Kết quả: Người dùng được chuyển đến trang xác nhận thanh toán (/checkout-step-two.html).

5. Kết quả đạt được

Tất cả các kịch bản kiểm thử đều chạy PASS

Cypress hoạt động ổn định và dễ sử dụng

Các chức năng chính của website được kiểm tra đầy đủ bằng kiểm thử tự động

Video và ảnh chụp màn hình kết quả được lưu lại làm minh chứng

6. Kết luận

Qua bài thực hành này, sinh viên đã nắm được cách cài đặt, cấu hình và sử dụng Cypress để thực hiện kiểm thử tự động End-to-End. Việc áp dụng Cypress giúp tiết kiệm thời gian kiểm thử, giảm lỗi thủ công và nâng cao chất lượng phần mềm. Đây là một công cụ hữu ích trong quá trình phát triển và đảm bảo chất lượng ứng dụng web.

7. Tài liệu tham khảo

Cypress Documentation: https://docs.cypress.io

Website kiểm thử: https://www.saucedemo.com
