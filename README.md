# Giới thiệu
Đồ án Kiểm thử phần mềm được thực hiện theo phương thức Kiểm thử tự động (Automation Testing) nhằm nâng cao hiệu quả kiểm thử và đảm bảo chất lượng phần mềm ở nhiều mức độ khác nhau.
Dự án bao gồm các loại kiểm thử như sau:

* Kiểm thử đơn vị (Unit Testing)
> - Áp dụng `White-box Testing`
> - Xây dựng các test case kiểm tra logic xử lý của bài toán hình chữ nhật trên hệ trục tọa độ Oxy bằng ngôn ngữ `C#`
> - Áp dụng `Data-Driven Testing`
> - Tự động đọc dữ liệu kiểm thử từ file CSV và Excel để thực thi nhiều bộ test khác nhau

* Kiểm thử chức năng tự động (Automated Functional Testing)
> - Áp dụng `Black-box Testing`
> - Thực hiện tự động hóa các luồng chức năng chính trên website thương mại điện tử [hoayeuthuong.com](https://hoayeuthuong.com) bằng `Selenium WebDriver`

* Kiểm thử API (API Testing)
> - Áp dụng `Integration Testing` và `Black-box Testing`
> - Kiểm tra và xác thực dữ liệu trả về từ các API [dummyjson.com](https://dummyjson.com/carts) công khai trên Internet. Sử dụng Postman để gửi request và viết test script `JavaScript` nhằm validate status code và response data.
> - Sử dụng JSON Server để tạo REST API giả lập phục vụ kiểm thử

# Công nghệ và công cụ sử dụng
* Ngôn ngữ: `C#`, `JavaScript`
* Framework kiểm thử: `Unit Test (.NET)`, `Selenium WebDriver`
* API Testing: `Postman`
* Quản lý mã nguồn: `GitHub`

# Phạm vi kiểm thử 
* Kiểm tra logic xử lý bài toán hình chữ nhật với chức năng tính diện tích và kiểm tra giao nhau giữa hai hình chữ nhật.
* Tự động hóa các chức năng của website thêm sản phẩm vào giỏ hàng, tìm kiếm sản phầm, liên kết trang mạng xã hội, chuyển ngôn ngữ.
* Kiểm tra API và xác thực dữ liệu trả về với các phương thức `GET`, `POST`, `PUT`, `DELETE`.

# Hướng dẫn cài đặt và bài báo cáo chi tiết
## Yêu cầu môi trường
* Visual Studio (khuyến nghị `2022` trở lên)
* .NET SDK (phiên bản `4.7.2` trở lên)
* Google Chrome
* ChromeDriver (phiên bản tương thích với Google Chrome)
* Postman
* Node.js (phiên bản `10.9.2` trở lên)
## Hướng dẫn cài đặt
- B1: Clone project [Automation_Testing](https://github.com/ChiHao144/automation-testing)
- B2: Mở file `.sln` bằng Visual Studio. Hệ thống sẽ tự động restore NuGet Packages.
- B3: Cấu hình `ChromeDriver` (đối với Selenium Test) đảm bảo phiên bản ChromeDriver khớp với phiên bản Google Chrome đang sử dụng.
- B4: Mở Test Explorer. Chọn Run All để chạy toàn bộ test.
- B5: Chạy API Test. Mở Postman, chạy các request và kiểm tra kết quả.
- B6: Cài đặt Json Server `npm install i json-server`. Dùng `cmd` tạo 1 file json nhập nội dung json, dùng lệnh `json-server –watch ten_file_json.json` để chạy sau đó click vào vào link `http://localhost:3000/` để truy cập API.
## Báo cáo chi tiết
Toàn bộ nội dung phân tích yêu cầu, thiết kế test case, mô tả kỹ thuật và hình ảnh minh họa được trình bày chi tiết trong file báo cáo đính kèm.
[File báo cáo chi tiết](https://github.com/ChiHao144/automation-testing/blob/master/DoAn_KTPM_StepByStep_52_Hao_54_Hieu.docx).
