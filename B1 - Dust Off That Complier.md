# 

Sau khi hoàn thành các bước cài đặt, bạn cần chắc chắn rằng nó được cài đặt đúng và sẵn sàng sử dụng. Các đơn giản nhất để kiểm tra là hãy chạy một chương trình `C` đơn giản sau đây


_ex1.c_
-----
```c
#include <stdio.h>

/* Đây là dòng chú thích */
int main(int argc, char *argv[]){
	int distance = 100;

	// đây là một dùng chú thích khác
	printf("You are %d mile away.\n", distance);

	return 0;
}
```
__Breacking It Down__
Có thể bạn đang không hiểu hết được những gì bạn đang viết. Tôi sẽ giải thích tất cả mọi thứ ở dưới đây:
- `include` sử đụng để chèn các thư viện đã được xây dựng sẵn vào trong chương trình của bạn. Các thư viện này có tên mở rộng là `.h` và nó chứa các function được sử dụng trong chương trình của bạn.
- `//` được sử dụng trong trường hợp bạn muốn chú thích chi tiết các dòng code của bạn. Các dòng này sẽ được lưu lại trong file code của bạn nhưng khi được đóng gói, complier sẽ bỏ qua. Trong trường hợp bạn có một dòng chú thích rất dài, và có nhiều dòng, hãy bắt đầu với `/*` và kết thúc bằng `*/`.
- Một phiên bản phức tạp của `main` function đã được sử dụng. Để một chương trình `C` hoạt động, bắt buộc phải có hàm `main`. Một hàm `main` đầy đủ luôn luôn trả về một số nguyên `int` và nhận lấy 2 tham số: một số nguyên `int` và một chuỗi `char *`. Chúng ta sẽ tìm hiểu về nó kỹ hơn về nó sau.
- Để bắt đầu phần nội dung của một hàm, `{` được sử dụng để đánh dấu sự bắt đầu. Với `Python`, chúng ra sử dụng `:` và ở một số ngôn ngữ khác, chúng ta sử dụng `begin` hoặc `do`
- Biến và phép gán có thể được sử dụng cùng một lúc. Đây là các để tạo ra một biến, `kiểu tên = giá_trị;`. Tất cả các dòng code sử dụng trong `C` bắt buộc phải có dấu kết thúc `;`
- `printf` là hàm được sử dụng để in nội dung lên màn hình. Giống như các hàm khác, các sử dụng là `tên(tham_số_1, tham_số_2);` hoặc chúng ta cũn có thể sử dụng nó mà không cần bất cứ tham số nào. 
- `return` được sử dụng để báo cho HĐH về gía trị kết thúc chương trình. Chúng ta sẽ cùng tìm hiểu thêm về các giá trị này.
- Cuối cùng là dấu báo kết thúc hàm: `}` và cũng là dấu báo kết thúc chương trình
Đó là tất cả thông tin trong dòng code vừa rồi, qua đây bạn có thể hiểu qua những gì đang xảy ra. Nếu còn điều gì chưa hiểu, bạn có thể đoán nó là gì trước khi chúng ta tiếp tục. 

__Những gì bạn sẽ thấy__
_Excercise 1 Session_
----
```
$ make ex1
cc     ex1.c   -o ex1
$ ./ex1
You are 100 miles away.
```
Command đầu tiên `make` là một công cụ để đóng gói chương trình `C`. Câu lệnh này sẽ tìm file `ex1.c` đóng gói nó thành chương trình tên là `ex1`. Vì `ex1` có thể chạy trược tiếp, nên bạn chỉ cần dùng câu lệnh tiếp theo để chạy.
__How to Break It__
Trong cuốn sách này, tôi sẽ cố gắng giúp bạn hiểu về các hiểu thêm về các dòng code của bạn. Hãy thử chạy chương trình với một số chỉnh sửa nhỏ. Hãy thử xoá một vài dòng code và chạy lai `make` bạn sẽ có lỗi xảy ra. Hãy thử đoán xem trong chương trình ở trên, những dòng code nào có thể xoá đi mà không dẫn đến lỗi chương trình.

__Bài Tập__
* Sửa lại code `ex1.c`, hãy thử xoá một vài dòng code và xem chuyện gì sẽ xảy ra.
* In thêm 5 dòng chữ phức tạp hơn 'hello world.'
* Chạy `man 3 printf` để tìm hiểu thêm về hàm `printf`
* Hãy thử viết một vài ký tự bạn không hiểu và đoán xem ý nghĩa của nó là gì. Chúng ta sẽ học thêm về các ký tự ở những bài tiếp theo và biết đâu, bạn đã có những dự đoán đúng.
