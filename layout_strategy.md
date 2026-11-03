# Báo cáo Phân tích Lựa chọn Thiết kế (Layout Strategy)

- **Nguyên tắc chủ đạo:** "CSS Grid sinh ra để làm Layout tổng thể, Flexbox sinh ra để làm Component chi tiết."
- **Navbar:** Sử dụng Flexbox (`display: flex; justify-content: space-between; align-items: center;`) giúp tự động co giãn theo nội dung, tránh lỗi tràn chữ khi đổi ngôn ngữ.
- **Dashboard:** Sử dụng CSS Grid (`display: grid; grid-template-columns: repeat(3, 1fr);`) giúp làm phẳng DOM (Shallow DOM), quản lý bố cục 2 chiều hiệu quả với `grid-row: span 2`.
- **Pricing:** Sử dụng hệ thống lưới 12 cột tiêu chuẩn của Bootstrap 5 (`row`, `col-12 col-md-4`) giúp hiển thị 3 cột trên Desktop và tự động xếp chồng trên Mobile mà không cần viết tay Media Queries phức tạp.