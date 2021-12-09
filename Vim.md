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

- Thao tác lệnh để xem nội dung file text:  
`cat [option] [filename]` (Lệnh cat-concatenate bản chất là ghép nối các file với nhau)  
Một số option sử dụng trong lệnh `cat` như sau:  

![image](https://user-images.githubusercontent.com/92737759/145425183-f17dafd6-18d4-45ca-99a2-9ec8815bc30e.png)

- Câu lệnh xem nội dung file theo nhiều cách hiển thị ( hệ bát phân, thập phân, thập lục phân, ASCII): `od [option] [filename]`

- Một số các công cụ lệnh khác:  
1. `split [option] [input [prefix]]`: Cắt các file lớn thành nhiều file nhỏ hơn  
  Ví dụ: ![image](https://user-images.githubusercontent.com/92737759/145430194-53621e3a-3478-4d0a-a468-44c8409d7418.png)
2. `tr [option] SET1 [SET2]`: Translate, dịch các chuỗi từ chữ hoa thành chữ thường  
  Ví dụ: `cat [filename] :tr "[A-Z]" "[a-z]"`
3. `sort [option] [filename]`: sắp xếp file theo ý muốn  
  Ví dụ: ![image](https://user-images.githubusercontent.com/92737759/145438578-3034b946-24c1-49c9-9627-2aa906009783.png)
4. `nl [option] [filename]`: Hiển thị STT các dòng  
  Ví dụ: ![image](https://user-images.githubusercontent.com/92737759/145439240-883c1d45-dce6-4b02-ac00-bbd68861df44.png)

- Các công cụ more, less, head, tail 
  Ví dụ: `tail -f [filename]`: xem file ở dạng realtime  
- Công cụ `wc [option] [filename]`: Đếm số dòng số byte... trong file text  

![image](https://user-images.githubusercontent.com/92737759/145442146-b27c9006-b081-4846-9cce-66841b251cc1.png)
- Công cụ `cut [option] [filename]`: sử dụng cho các file có cấu trúc (Được chia thành các cột riêng và ta có thể truy xuất dữ liệu vào từng trường cụ thể)  

![image](https://user-images.githubusercontent.com/92737759/145442722-1e9e4b03-a774-4abe-acb1-d0e147eda973.png)

  Ví dụ: ![image](https://user-images.githubusercontent.com/92737759/145443260-e108ee94-e2d7-4349-9826-bc0f1142d2a8.png)
