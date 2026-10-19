Phần 1 – Phân tích
1. Hàng tiêu đề bị Merge Cell → vi phạm quy tắc không merge ô.
2. Hàng 6 bị trống → vi phạm quy tắc không có hàng trống.
3. Cột Trạng thái có ```hỏng``` và ```Hỏng```/có khoảng trắng → dữ liệu không đồng nhất, Filter tách thành 2 nhóm.

Phần 2 – Sửa
- Gỡ Merge Cell.
- Xóa hàng 6.
- Dùng ```TRIM()``` để xóa khoảng trắng thừa:
```
Excel

=TRIM(E2)
````

- Chuẩn hóa thành cùng một giá trị, ví dụ “Hỏng”.
- Chọn toàn bộ bảng →``` Ctrl + Shift + L``` → lọc Trạng thái = Hỏng.

Sau khi sửa, Filter sẽ lọc tất cả thiết bị hỏng trong một nhóm.
