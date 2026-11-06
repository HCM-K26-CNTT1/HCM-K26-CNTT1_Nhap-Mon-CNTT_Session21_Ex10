# BÀI 10: ĐÁNH GIÁ ĐA GIẢI PHÁP QUY TRÌNH KHẮC PHỤC SỰ CỐ KỸ THUẬT

## PHẦN 1. SO SÁNH HAI PHƯƠNG ÁN

### 1.1. Bảng so sánh

| Tiêu chí                  | Phương án 1: Hỗ trợ cảm tính                       | Phương án 2: Troubleshooting 4 chặng           |
| ------------------------- | -------------------------------------------------- | ---------------------------------------------- |
| 1. Thời gian xử lý        | Lâu vì phải chờ kỹ sư trả lời.                     | Nhanh hơn vì KTV có thể tự tìm cách sửa lỗi.   |
| 2. Chi phí cho Senior Dev | Cao vì phải giải quyết nhiều lỗi nhỏ.              | Thấp hơn vì chỉ hỗ trợ những lỗi khó.          |
| 3. Năng lực KTV           | Phụ thuộc vào người khác, không biết tự xử lý lỗi. | Biết tìm kiếm, phân tích và tự sửa lỗi cơ bản. |
| 4. Lưu trữ kiến thức      | Tin nhắn dễ bị trôi, khó tìm lại.                  | Lỗi được ghi lại để mọi người cùng tham khảo.  |

### 1.2. Kết luận lựa chọn

Em chọn Phương án 2 – Troubleshooting 4 Chặng vì:

- Giúp giảm thời gian trạm sạc bị ngừng hoạt động.
- Tiết kiệm thời gian cho các kỹ sư cấp cao.
- Giúp kỹ thuật viên biết tự tìm và sửa lỗi.
- Lưu lại lỗi cũ để tránh gặp lại mà không biết cách xử lý.

Khi mở rộng lên 1.000 trạm sạc, công ty không thể để mọi lỗi đều phải chờ kỹ sư cấp cao giải quyết. Vì vậy, phương án 2 phù hợp và hiệu quả hơn.

## PHẦN 2. SƠ ĐỒ QUY TRÌNH GỠ LỖI

### 2.1. Sơ đồ Decision Flowchart

```
       BẮT ĐẦU
           |
           v
    Kiosk xuất hiện lỗi
           |
           v
  CHẶNG 1: TÌM KIẾM GOOGLE
  - Bóc tách từ khóa lỗi
  - Dùng site:, "..." và -
           |
           v
  CHẶNG 2: ĐỌC STACKOVERFLOW
          / GITHUB
  - Đọc lướt khoảng 30 giây
  - Kiểm tra tích xanh, Upvote
           |
           v
    Sửa được lỗi chưa?
       /       \
     Có        Chưa
     |           |
     v           v
   Kết thúc   CHẶNG 3: HỎI AI
              - Gửi nội dung lỗi
              - Nhờ giải thích tiếng Việt
              - Xin 2 cách sửa lỗi
                   |
                   v
              Thử 2 cách trong
                 15 phút
                   |
                   v
              Sửa được lỗi chưa?
                /       \
              Có        Chưa
              |           |
              v           v
            Kết thúc  CHẶNG 4:
                      LẬP BUG REPORT
                      - Ghi tên lỗi
                      - Ghi môi trường
                      - Ghi cách xảy ra lỗi
                      - Đính kèm ảnh/log lỗi
                            |
                            v
                      Gửi IT Helpdesk
                            |
                            v
                         KẾT THÚC
```

### 2.2. Giải thích 4 chặng

- Chặng 1: Tìm lỗi trên Google bằng từ khóa và các toán tử tìm kiếm để có kết quả chính xác hơn.
- Chặng 2: Đọc các bài viết trên StackOverflow hoặc GitHub để tìm cách sửa lỗi đã có người gặp trước đó.
- Chặng 3: Nếu chưa hiểu lỗi thì hỏi AI giải thích bằng tiếng Việt và hướng dẫn 2 cách khắc phục.
- Chặng 4: Nếu thử vẫn không được sau 15 phút thì lập Bug Report, gửi IT Helpdesk để được hỗ trợ.

## PHẦN 3. KẾT LUẬN

Theo em, VoltCharge nên chọn phương án 2 vì giúp kỹ thuật viên chủ động xử lý lỗi, giảm thời gian chờ đợi và tiết kiệm chi phí cho công ty. Ngoài ra, việc ghi lại các lỗi đã gặp giúp nhân viên có kinh nghiệm hơn và công ty dễ dàng mở rộng lên 1.000 trạm sạc.
