# PHẦN 1: PHÂN TÍCH BÀI TOÁN
## 1. Xác định Đầu vào & Đầu ra

-   **Đầu vào (Inputs):**
     -  **Nhân sự (4 nhóm/vai trò):** Ban Kỹ thuật (3 người), Ban Thiết kế (2 người), Ban Kinh doanh (2 người), Nhà đầu tư tiềm năng (1 người ngoài tổ chức).
     - **Tài liệu:** Mã nguồn/API keys, Tài sản UI/đồ họa, Business Plan, Slide Pitch, Tài liệu chung/Chung của dự án.
     - **Chính sách bảo mật:** 5 nguyên tắc Google Drive (Tối thiểu quyền, Chống rò rỉ, Cộng tác, Version history tối thiểu 30 ngày, Hết hạn tự động).
- **Đầu ra (Outputs):**
   - Bảng phân quyền chi tiết cho từng vai trò đối với từng loại tài liệu.
   - Giải pháp xử lý các "bẫy dữ liệu" và quy trình xử lý nhân sự nghỉ việc.

## 2. Đề xuất giải pháp
- **Cấp 1: dự án**
    - Thư mục quản lý chung toàn bộ dự án: Trưởng nhóm
- **Cấp 2: ban nhóm**
     - Tài liệu chung, kế hoạch làm việc: cả nhóm
     - Thư mục riêng của Ban Kỹ thuật: Code, API, Test
     - Thư mục riêng của Ban Thiết kế: UI, Graphics
     - Thư mục riêng của Ban Kinh doanh: Business Plan, tài chính
     - Thư mục dùng chung để gọi vốn cho Nhà đầu tư: Slide thuyết trình kêu gọi

## 3.Thiết kế:
- Bước 1: tạo thư mục chung bao quát cả project
- Bước 2: đặt tên các phân cấp
    + Ban kỹ thật
    + Ban thiết kế
    + Ban kinh doang
    + Ban tìm kiếm nhà tư
 - Bước 3: quyền truy cập
    + Ban kỹ thật: quyền chỉnh sửa
    + Ban thiết kế: quyền chỉnh sửa
    + Ban kinh doanh: quyền xem 
    + Ban tìm kiếm nhà tư: quyền xem
- Bước 4: Kiểm tra
   + Check lại project sau khi các ban đảm nhiệm
   + Chốt dự án
- Bước 5: thu hồi và cập nhật
    + Cài đặt thời gian truy cập cho nhà đầu tư trong vòng 14 ngày
    + Thu hồi quyền truy cập ngay khi có biến động nhân sự

# Phần 2 : Triển khai & chống lỗi
## 4. Bảng phân chia
|Loại tài liệu|Ban KT|Ban TK| Ban KD|Nhà đầu tư|Ghi chú bảo mật|
|:---:|:---:|:---:|:---:|:---:|:---:|
|Tài liệu chung|viewer|viewer|viewer|viewer|dữ liệu tham khảo chung của dự án|
| API Keys|editor|no access|no access|no access|dữ liệu bảo mật tuyệt đối|
|UI/đồ họa|viewer|editor|viewer|viewer|thiết kế giao diện của người dùng|
|Business Plan|viewer|no access|editor|viewer|Chứa thông tin chiến lược, hạn chế sửa bậy|
|Slide Pitch|viewer|viewer|viewer|editor|viewer|
## 5.Bẫy dữ liệu
- Bẫy 1: cấp quyền viewer cho họ xem chứ không cấp quyền chỉnh sửa vì đây không phải chuyên môn của họ
- Bẫy 2: cấp quyền viewer cho nhà đầu tư vì quyền viewer có thể xem và tải PDF về
- Bẫy 3: 
   + Thu hồi quyền truy cập của thành viên nghỉ
   + Chặn và vô hiệu hóa tài khoản mà thành viên từng tham gia project
   + Check lịch sử truy cập project để xen những lần truy cập hàng ngày để đẩy cao tính bảo mật 

