# XS Vietlott Lab

Bản kiểm duyệt ứng dụng phân tích thống kê cho Mega 6/45, Power 6/55 và Lotto 5/35.

## V1 · Forward Test 01

- Đồng bộ hai nguồn dữ liệu cộng đồng, bổ sung bản ghi mới nhất từ kho đối chiếu với Vietlott và bỏ qua bộ nhớ đệm của trình duyệt.
- Tự kiểm tra dữ liệu khi mở lại app, khi quay về từ màn hình nền và mỗi 5 phút trong lúc app đang mở.
- Phân tích 100 kỳ: tần suất, nóng/lạnh/quá hạn, tổng, chẵn/lẻ và phân bố theo khoảng.
- Giao thức V1 cố định: cửa sổ 100 kỳ, chiến lược tổng hợp cân bằng và 5 bộ dự báo mỗi kỳ.
- Khi lưu, hệ thống khóa thêm 15 bộ đối chứng cùng thời điểm: random đều, random có cấu trúc và chọn theo tần suất.
- Chỉ đối chiếu dự báo sau khi xuất hiện kết quả mới; bản ghi đã đối chiếu được bảo vệ khỏi xóa.
- Báo cáo forward test theo dõi số mẫu, phân phối số trùng, khoảng tin cậy, p-value và hiệu quả từng baseline.
- Lịch sử được lưu bằng `localStorage` trên thiết bị đang sử dụng.

> Đây là công cụ mô tả và kiểm định thống kê. Không có chiến lược nào bảo đảm trúng thưởng.

## Chạy thử

Mở `index.html` hoặc chạy một máy chủ tĩnh trong thư mục dự án.
