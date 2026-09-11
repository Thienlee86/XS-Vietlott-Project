# XS Vietlott Lab

Bản kiểm duyệt ứng dụng phân tích thống kê cho Mega 6/45, Power 6/55 và Lotto 5/35.

## V2 · Budget Test 01

- Đồng bộ hai nguồn dữ liệu cộng đồng, bổ sung bản ghi mới nhất từ kho đối chiếu với Vietlott và bỏ qua bộ nhớ đệm của trình duyệt.
- Tự kiểm tra dữ liệu khi mở lại app, khi quay về từ màn hình nền và mỗi 5 phút trong lúc app đang mở.
- Mỗi dự báo được gắn với ngày quay mục tiêu; chỉ kết quả đúng ngày đó mới được phép đối chiếu.
- Phân tích 100 kỳ: tần suất, nóng/lạnh/quá hạn, tổng, chẵn/lẻ và phân bố theo khoảng.
- Giao thức V2 cố định: cửa sổ 100 kỳ và đúng 2 bộ mỗi kỳ theo ngân sách thực tế.
- Bộ thứ nhất ưu tiên điểm tổng hợp; bộ thứ hai giảm trùng lặp để mở rộng độ phủ.
- Khi lưu, hệ thống khóa thêm 6 bộ đối chứng cùng thời điểm: 2 random đều, 2 random có cấu trúc và 2 chọn theo tần suất.
- Lịch sử V1 vẫn được giữ và báo cáo tách theo phiên bản để tránh trộn ngân sách 5 bộ với 2 bộ.
- Theo dõi chi phí, tiền trúng nhập thực tế và ROI của riêng V2.
- Chỉ đối chiếu dự báo sau khi xuất hiện kết quả mới; bản ghi đã đối chiếu được bảo vệ khỏi xóa.
- Báo cáo forward test theo dõi số mẫu, phân phối số trùng, khoảng tin cậy, p-value và hiệu quả từng baseline.
- Lịch sử được lưu bằng `localStorage` trên thiết bị đang sử dụng.

> Đây là công cụ mô tả và kiểm định thống kê. Không có chiến lược nào bảo đảm trúng thưởng.

## Chạy thử

Mở `index.html` hoặc chạy một máy chủ tĩnh trong thư mục dự án.
