# Công cụ Editing text file trong linux
### Có 3 công cụ phổ biến: 
1. Emacs (Nền tảng mã nguồn mở), có rất nhiều tính năng đa dạng khác nhau
2. Nano (Thiết kế đơn giản, dễ sử dụng)
3. Vim (Công cụ phổ biến nhất)  

> ### Vim
> 
![image](https://user-images.githubusercontent.com/92737759/145265292-a4076ea8-3b58-4947-9791-0982d81a71c6.png)
- Cấu trúc Vim có 3 loại mode: Command Mode, Input Mode và Last Line Mode
1. Command Mode: Là command trung gian giữa 2 mode còn lại. Khi ta mở trình soạn thảo Vim sẽ vào command mode, tại mode này không thể cập nhật viết văn bản. Nhấn phím i (insert) hoặc a (append) để vào mode input
2. Input mode: Nơi ta có thể thao tác viết text. Nếu muốn thoát ra mode command, nhấn phím Escape
3. Last line mode: Nơi ta thực hiện các tác vụ như lưu file, thoát khỏi vim. Nhấn phím ":" và return để vào hoặc thoát ra mode last line
- Các thao tác lệnh cơ bản trong vim  

![image](https://user-images.githubusercontent.com/92737759/145266627-6003f2f3-7007-45e7-aaf5-05eaa4abba5a.png)  

![image](https://user-images.githubusercontent.com/92737759/145266817-a607d024-0445-4c42-97fb-943cc0ba7317.png)
- Các câu lệnh sử dụng trong command mode  

![image](https://user-images.githubusercontent.com/92737759/145267136-42a83b8a-fcbf-4ae3-bdee-00441409fcb0.png)
  + u: Khôi phục lại các dòng vừa xóa
  + Thao tác lặp lệnh. Ví dụ: 4 + dd (Xóa 4 dòng)
  + Thoát khỏi file: Nhấn "wq!", hoặc "x" hoặc "q!"
  + Đứng từ flie vim đọc, ghi các file khác mà không cần thoát ra ngoài: "! ls", "r! ls"
  + Câu lệnh đặt các số đầu dòng text để dễ dàng quản lý, ra soát lỗi: set number
