# PHẦN 1: THIẾT KẾ HYBRID WORKFLOW

1.  **Mất file Slide:**  Không xảy ra, vì Auto Sync đã tự động đồng bộ ngầm bản mới nhất lên Cloud.
    
2.  **3 bước Auto Sync:** Tải ứng dụng Cloud -> Đăng nhập và chọn thư mục đồng bộ -> Di chuyển file vào thư mục.
    
3.  **Khôi phục file Word:** Mở file   `File`  ->  `Version history`  -> Chọn mốc thời gian trước đó ->  `Restore`.
    
4.  **Xử lý 2 sai lầm:**
    
    -   Thư mục `node_modules`: Cho vào danh sách bỏ qua (Ignore list) vì có thể cài lại bằng lệnh.
        
    -   Phim 4K: Chuyển ra ngoài, không lưu vào thư mục dự án chung.
        

# PHẦN 2: PHÂN QUYỀN CHIA SẺ AN TOÀN

1.  **Bảng phân quyền:**
    |File|Mức quyền|Phạm vi chia sẻ|Giải thích|
    |:---:|:---:|:---:|:---:|
    |`BaoCao_CuoiKy_SmartCampus.docx` gửi giảng viên | Viewer | Restricted (Chỉ email GV) | Chấm điểm, không cho sửa|
    |`Slide_BaoCao.pptx` cho 5 thành viên nhóm|Editor | Restricted (5 người) | Cùng làm việc gấp|
    |`GopY_BanNhap.docx` gửi anh khóa trên|Commenter | Restricted (Chỉ email anh) | Nhận xét không sửa trực tiếp|
    |`ThongTin_CaNhan_NhomVien.xlsx`|Restricted (Chỉ nội bộ) | Restricted (Nội bộ) | Bảo mật CCCD/SĐT|
        
2.  **Quy tắc Cờ Đỏ:** Tuyệt đối không kết hợp `Anyone with the link` + `Editor` cho file chứa dữ liệu nhạy cảm để tránh lộ thông tin.
    
3.  **Settings của Slide:** Chặn Editor không được tự ý đổi quyền/mời người ngoài và chặn tải/in/sao chép nếu cần thiết.

# PHẦN 3: TỔ CHỨC GIAO TIẾP NHÓM

1.  **3 vấn đề:** Mắc lỗi No-Hello, spam tin nhắn giải trí, dùng `@all` lúc nửa đêm gây áp lực.
 2.  **Tên Channel:**  
- Kênh thông báo chung
- Kênh thảo luận chuyên môn
3.  **Viết lại tin nhắn của Lan (Asynchronous):**  "Mình đang gặp lỗi API đăng nhập (chi tiết ở ảnh đính kèm). Ai rảnh lúc nào xem giúp mình nhé, không gấp đâu ạ!"
4.  **Viết lại tin nhắn Trưởng nhóm:** Dùng **Schedule Send** (hẹn 8h sáng) và đổi `@all` thành tag đích danh:  "@Nam và @Lan kiểm tra lại phần việc giúp mình nhé!"

# PHẦN 4: THÔNG BÁO TỔNG HỢP
"Chào buổi sáng đội nhà mình nhé, mình xin cập nhật tiến độ:
1. Đã bật **Auto Sync** toàn bộ thư mục dự án để chống mất file.
2. Đã gửi file báo cáo cho Giảng viên ở chế độ **Viewer / Restricted** an toàn.
3.  @Nam và @Lan ơi, hai bạn kiểm tra lại phần việc còn thiếu giúp nhóm nhé!"
