# 1. CLI là gì?
Nói một cách đơn giản, CLI là viết tắt của giao diện dòng lệnh. Nó là một chương trình cho phép người dùng gõ các lệnh văn bản hướng dẫn máy tính thực hiện các công việc cụ thể.  

# 2. Rễ của CLI
 
Trong những năm 1960, CLI được sử dụng rộng rãi.  

Khi màn hình máy tính chỉ có thể hiển thị thông tin văn bản thì các hệ điều hành như MS-DOS sử dụng CLI làm giao diện người dùng tiêu chuẩn.

Về cơ bản, người dùng phải nhập một lệnh trên CLI để thực hiện các tác vụ, vì đây là cách duy nhất để giao tiếp với máy tính.  

Sau khi nhập một lệnh, kết quả mà người dùng nhận được sẽ là thông tin văn bản hoặc hành động cụ thể do máy tính thực hiện. Điều đó đang được nói, gõ đúng lệnh là chìa khóa.  

Nếu người dùng gõ sai lệnh, rất có thể họ sẽ xóa nhầm tệp hoặc vô tình đóng chương trình trước khi lưu công việc của họ. Đây là những gì mọi người coi là nhược điểm chính của việc sử dụng CLI.  

# 3. Shell- nền tảng đằng sau CLI
Nếu chúng ta đi sâu từ CLI vào phần sâu hơn của hệ điều hành, chúng ta sẽ tìm thấy shell.  

Shell là một giao diện người dùng chịu trách nhiệm xử lý tất cả các lệnh được nhập trên CLI. Nó đọc và diễn giải các lệnh và hướng dẫn hệ điều hành thực hiện các tác vụ theo yêu cầu.  

Nói cách khác, shell là một giao diện người dùng quản lý CLI và hoạt động như người trung gian, kết nối người dùng với hệ điều hành.  

Trong thực tế, có nhiều thứ mà shell có thể xử lý, chẳng hạn như:  

* Làm việc với các tệp và thư mục  
* Mở đầu và kết thúc chương trình  
* Quản lý các quy trình máy tính  
* Thực hiện các công việc lặp đi lặp lại  

Trong số nhiều loại shell, phổ biến nhất là Windows shell (dành cho Windows) và bash (dành cho Linux và MacOS).
> ## Window shell
> 
Vỏ mặc định trong Windows là **CMD.exe** hoặc **Command Prompt** . Trên thực tế, Microsoft đã sử dụng **Command Prompt** từ ngày xưa, nơi **MS-DOS** là hệ điều hành chính.  

Để mở Command Prompt, bạn có thể nhấp vào **Start -> All Programs -> Accessories -> Command Prompt**. Hoặc, bạn có thể chỉ cần nhấn **Windows + R** , sau đó nhập **CMD** và nhấn *enter* .  

Command Prompt có thể quản lý nhiều thứ trong hệ điều hành Windows :  

- Thay đổi thư mục, danh sách thư mục, nội dung, v.v.  
- Xử lý mạng như hiển thị cài đặt mạng IP  
- Quản lý tệp như đổi tên, di chuyển, v.v.  
- Quản lý phương tiện như định dạng và đổi tên tập  

Một số cú pháp khác:  

* Thay đổi thư mục  

Để điều hướng đến một thư mục hoặc thư mục cụ thể trong dấu nhắc lệnh, hãy sử dụng **CD [đường dẫn]** . Ví dụ: `CD C: \ Program Files`  

* Đổi tên tệp  

Để đổi tên tệp trong một thư mục cụ thể, hãy sử dụng **REN [drive:] [path] [source] [target]** . Nếu bạn đề cập đến vị trí, điều đó có nghĩa là tệp đã đổi tên sẽ được lưu trong cùng một thư mục. Ví dụ:
`REN d: unsitled.txt unsitled1.txt`  
* Xóa tệp  

Để xóa tệp trong dấu nhắc lệnh, hãy sử dụng **DEL [tên tệp]**. Ví dụ: `DEL / F unsitled.txt`  

* Đổi tên ổ đĩa

Để chỉnh sửa tên của ổ đĩa khối lượng cụ thể, hãy sử dụng **LABEL [drive:] [tên ổ đĩa mới]**.Có thể sử dụng tối đa 32 ký tự trên ổ đĩa NTFS và 11 ký tự trên ổ đĩa FAT. Ví dụ: `D: \> LABEL d: MyData`  

> # Bash
> 
Bash là viết tắt của **Bourne Again Shell** và được phát triển bởi **Free Software Foundation** .  

Bash là một loại shell được sử dụng trong **MacOS** và nhiều bản phân phối **Linux**. Tuy nhiên, bạn cũng có thể cài đặt bash Linux trên Windows 10.  

Trong Linux, Bash shell là một trong nhiều shell mà người dùng Linux có thể sử dụng. Các loại khác là **Tchs shell , Ksh shell và Zsh shell** .  

Trong hầu hết các bản phân phối Linux, nếu bạn sử dụng Gnome desktop, tên là Terminal , nhưng nếu bạn sử dụng KDE , tên là Konsole .  

Trong khi đó, trong MacOS, chương trình là Terminal.app . Để chạy chương trình này, **Application -> Utilities -> Terminal**. Hoặc, bạn có thể chỉ cần nhập thiết bị đầu cuối bằng cách sử dụng tìm kiếm Spotlight.   

Sau khi thiết bị đầu cuối được mở, bạn có thể bắt đầu nhập lệnh. Về cơ bản, hầu hết các lệnh bao gồm: lệnh, đối số và tùy chọn .  

Trong khi lệnh chứa lệnh mà chúng ta muốn thực hiện, đối số cho biết lệnh sẽ hoạt động ở đâu và tùy chọn yêu cầu sửa đổi đầu ra.  

Để bắt đầu, bạn cần biết cú pháp để xử lý shell. Đây còn được gọi là shell script - cách sử dụng script trong CLI để chạy các tác vụ nhất định.  

Mặc dù có nhiều lệnh bạn có thể sử dụng với CLI, nhưng tất cả chúng đều thuộc hai loại :  

* Các lệnh xử lý các quy trình  
* Các lệnh xử lý tệp  
