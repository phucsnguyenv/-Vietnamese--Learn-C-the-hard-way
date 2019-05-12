# Hướng dẫn cài đặt 
C là một loại ngôn ngữ lập trình bậc thấp, thường được sử dụng trong lập trình di động, ứng dụng máy tính và các thiết bị vi điện tử. 

Bài tập này sẽ hướng dẫn các bạn cài đặt môi trường để complie code C thành một chương trình

## Trên Linux
Linux được xem là môi trường thân thiện nhất dùng để cấu hình và phát triển phần mềm sử dụng C. Với Debian, sử dụng câu lệnh sau để cài đặt
*REQUIRED* Máy tính của bạn cần có kết nối Internet
```bash
$ sudo apt-get install build-essential
```
Với RPM based như Fedora, RedHat hay Centros
```bash
$ sudo yum groupinstall development-tools
```
Nếu ban đang sử dụng một phiên bản khác, hãy thử tìm kiếm trên trang chủ để tìm hiểu cách cài đặt. Sau khi đã cài đặt được `C complier`, hãy thử kiểm tra bằng câu lệnh sau đây
```bash
$ cc --version
```

## Trên Mac OS X
Cài đặt `C complier` trên MacOS cũng khá đơn giản. Hãy mở `Terminal` trên Mac và sử dụng câu lệnh sau
```bash
$ gcc
```
Câu lệnh sẽ hiện lên thông báo yêu cầu cài đặt `Xcode` bạn chỉ cần chọn cài đặt là được. Sử dụng `cc --version` để kiểm tra sau khi quá trình cài đặt `Xcode` hoàn tất.

## Windows
Hầu hết đối với các bạn sử dụng Windows thường cài `Dev C++` để complie cũng như edit code C của mình. Đây cũng là công cụ được khuyến nghị sử dụng trong môi trường đại học. Nhưng trong các bài tập này, tôi khuyên bạn nên sử dụng `Cygwin` đây là một chương trình mang nhiều đặc điểm của một hện thống UNIX. Phần mềm này cũng rất dễ cài đặt và sử dụng.Ngoài ra bạn có thể sử dụng `MinGW`
Bạn cũng có thể sử dụng `VirtualBox` để cài đặt một hệ thống Linux trên chính máy ảo bạn đang sử dụng. Đây cũng là một cách để bạn có thể học thêm về Linux một kỹ đăng chắc chắn sẽ rất hữu ích trong tương lại của bạn.

## Chương trình chỉnh sửa code
Chương trình chỉnh sửa code hay còn gọi là text editor, là một công cụ không thể thiếu và cũng cần được lựa chọn một cách có chủ ý. Vì đây là phần mềm bạn sẽ sử dụng hàng ngày trong quá trình viết code, không chỉ về tính năng, hiệu năng và còn là giao diện khiến bạn cảm thấy thoải mái nhất. Một liều quan trong bạn cần lưu ý, text editor không phải là complier, không có tính năng đóng gói code, đây chỉ là công cụ giúp bạn viết và chỉnh sửa code giống như `notepad` trên windows mà thôi. 
Một số công cụ bạn có thể thử qua: 
- Sublime text
- Notepad++
- Nano
- Emacs

## Hãy cân nhắc trong việc sử dụng IDE
__Warning!__
```
	Hãy tránh việc sử dụng `intergrated develop environment (IDE)` trong quá trình học tập một ngôn ngữ lập trình. IDE hữu ích trong việc hoàn thành code của bạn, nhưng nó lại không mang lại nhiều hiệu quả trong việc học tập. Với kinh nhiệm của tôi, những lập trình viên chuyên nghiệp thường không sử dụng IDE và họ không gặp bất kỳ vấn đề gì trong việc phát triển phần mềm của mình. Tôi cũng nhận ra rằng các đoạn code  được phát hành khi sử dụng IDE cũng có chất lượng thấp hơn. Tôi không dám chắc đâu là vấn đề, nhưng nếu bạn thật sự muốn học và phát triển kỹ năng của mình một cách chắc chắn, hãy cố gắng không sử dụng IDE trong quá trình học tập.
	Biết các sử dụng các phần mềm chỉnh sửa code chuyên nghiệp là một kỹ đăng hữu ích trong cuộc sống hiện đại. Khi bạn bị phụ thuộc vào IDE, bạn cần chờ IDE được phát hành trước khi bạn muốn học một ngôn ngữ mới. Sử dụng IDE cũng tiêu tốn khá nhiều thời gian của bạn. Thay vì phải cấu hình IDE để sử dụng một ngôn ngữ nào đó, bạn có thể code bất kỳ ngôn ngữ nào, bất kỳ khi nào bạn muốn mới text editor.

```