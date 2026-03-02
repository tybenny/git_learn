## 3. Hiển thị trạng thái với `git status`

Câu lệnh này sẽ hiển thị

- Bạn đang ở branch nào
- Trạng thái branch của bạn so với origin như thế nào (điều này đôi khi không chính xác vì dữ liệu đã được thay đổi trên origin, nên dùng `git fetch` để tải về dữ liệu mới nhất)
- Trạng thái các file trong dự án, file nào đang được git track (theo dõi)

```bash
git status
```

## 4. Các khu vực làm việc với Git

Dưới đây là các khu vực làm việc theo thứ tự:

1. **Khu vực làm việc**: Là nơi chúng ta đang code, vẫn ở local
2. **Khu vực staging**: Sau khi dùng `git add` thì file sẽ được đưa lên khu vực này, vẫn ở trên local
3. **Khu vực commited**: Sau khi dùng `git commit` thì file từ staging sẽ được đưa lên đây, vẫn ở trên local
4. **Khu vực remote (gọi là origin cũng được)**: Sau khi dùng `git push` thì sẽ đẩy file ở commited lên đây, bây giờ file đã được đưa lên server

## 5. Thêm file vào khu vực Staging với `git add`

Câu lệnh dưới đây sẽ thêm một hoặc nhiều file (đã thay đổi) vào khu vực **Staging**