Session04-Ex02
-Sửa nội dung lên master
- Đã cập nhật nội dung mới lên trên nhánh feature-update

## Báo cáo giải quyết Merge Conflict
1. Chuyển sang nhánh `master` và chỉnh sửa nội dung trong file `README.md`.
2. Chuyển lại quá trình merge nhánh `feature-update` vào `master` bằng lệnh:
   `git merge feature-update`

3. Git phát hiện xung đột do hai nhánh cùng chỉnh sửa một dòng trong file `README.md`.
4. Mở file `README.md` và xử lý xung đột thủ công bằng cách:
    * Xóa các ký hiệu `<<<<<<< HEAD`, `=======`, `>>>>>>> feature-update`.
    * Giữ lại và kết hợp nội dung phù hợp từ cả hai nhánh.

5. Lưu file sau khi giải quyết xung đột.
6. Đưa file đã giải quyết vào Staging Area:
   `git add README.md`

7. Tạo Merge Commit:
   `git commit -m "Resolve merge conflict"`

8. Kiểm tra lịch sử nhánh bằng:
   `git log --graph --oneline`
