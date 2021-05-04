## Tóm tắt sở lược về từng chương:

### Chương 1: Bạn đã sẵn sàng thúc đẩy phát triển phần mềm của mình chưa?

Bạn có muốn một ngôn ngữ đơn giản, biên dịch nhanh? Chạy nhanh? Dễ dàng phân phối cho người sử dụng? Bạn đã sẵn sàng học Go? Go là một ngôn ngữ tập trung vào sự đơn giản và tốc độ. Nó đơn giản hơn so với ngôn ngữ khác, nhanh chóng để học. Và nó giúp bạn tận dụng được vi xử lý đa luồngg của máy tính, vì thế chương trình chạy nhanh hơn. Chương này sẽ cho bạn thấy tất cả tính năng của Go làm cho cuộc sống developer của bạn trở nên dễ dàng hơn, làm bạn cảm thấy yêu đời hơn.

`------`

### Chương 2: Mỗi chương trình đểu có những phần chỉ áp dụng trong một số trường hợp nhất định.

Đoạn code này nên chạy nếu có một lỗi. Ngược lại đoạn code khác nên chạy. Hầu hết chương trình chứa mã chỉ được chạy khi một điều kiện nhất định là đúng. Vì thế hầu hết ngôn ngữ lập trình đều cung cấp cấu trúc điều kiện, điều dó cho phép bạn xác định đoạn mã có chạy hay không. Go cũng không ngoại lệ.

Bạn có thể cần một phần của code lặp lại nhiều lần. Giống hầu hết các ngôn ngữ, Go cũng cấp vòng lặp để chạy đoạn code nhiều hơn một lần. Chúng ta sẽ sử dụng cả hai trong chương này.

`------`

### Chương 3: Bạn đã bỏ lỡ.

Bạn sẽ gọi những `function` theo cách của chuyên gia. Nhưng chức năng duy nhất bạn có thể gọi, Go sẽ khai báo cho bạn. Bây giờ đến lượt của bạn. Chúng tôi sẽ chỉ bạn làm cách nào để tạo ra function của bạn. Chúng ta sẽ học cách khai báo function có và không có `parameters`. Chúng ta sẽ khai báo `function` trả về một giá trị, và học cách trả về nhiều giá trị vì thế chúng ta có thể biết khi nào xảy ra lỗi. Và chũng ta cũng sẽ học về `pointers`, thứ cho phép chúng ta sử dụng bộ nhớ một cách hiệu quả khi gọi những `functions`.

`------`

### Chương 4: Giờ là thời gian để tổ chức.

Cho đến giờ, chúng ta đang tập hợp tất cả code ở trong cùng 1 file. Khi chương trình chúng tôi phát triển lớn hơn và phức tạp hơn, điều đó sẽ nhanh chóng trở thành mớ hỗn độn.

Ở chương này, chúng tôi sẽ chỉ bạn cách tạo ra `packages` để giữ code liên quan đến nhau ở cùng một nơi. Nhưng `packages` tốt cho nhiều thứ hơn là chỉ việc tổ chức. `Packages` là cách dễ dàng dể có thể chia sẻ code giữa các chương trình của bạn. Và nó cũng là cách để chia sẽ code với các developer khác.

`------`

### Chương 5: Cách thức lưu trữ danh sách trong Go.

Danh sách địa chỉ, danh sách danh bạ, danh sách sản phẩm. Go có hai cách để lưu danh sách. Chương này sẽ giới thiệu `arrays` trước. Bạn sẽ học được cách tạo một `arrays`, làm đẩy `arrays`, lấy ra dữ liệu từ nó. Sau đó bạn sẽ học cách xử lý với toàn bộ phần tử của `arrays`. Cách khó hơn với vòng lặp `for`, cách dễ hơn với vòng lặp `range (...)`

`------`

### Chương 6: Chúng ta đã học, chúng ta không thể thêm phần tử vào một arrays được.

Nó chính là vấn đề thực tại của lập trình, bởi vì chúng ta không biết trước có bao nhiêu phần mà dữ liệu của tệp chúng ta chứa đựng. Nhưng đó là thứ mà `Go Slices` xuất hiện. `Slices` là một bộ sưu tập các loại có thể tăng để giữ những item thêm vào, điều này giúp sửa chữa chương trình hiện tại của chúng ta. Chúng ta cũng nhìn thấy `Slice` đưa ra cho người dùng một cách dễ dàng hơn để cung cấp dữ liệu cho tất cả chương trình của mình. và cách nó giúp bạn viết những function tiện lợi hơn khi gọi.

`------`

### Chương 7: Quăng mọi thứ thành đống cũng không sao cho đến khi bạn cần tìm lại thứ gì đó.

Bạn đã sẵn sàng tạo ra một danh sách giá trị sử dụng `arrays` và `slices`. Bạn đã thấy cách áp dụng cùng một thao tác cho mọi giá trị trong một `arrays` hoặc `slices`. Nhưng nếu bạn cần làm việc với giá trị cụ thể. Để tìm nó, bạn sẽ bắt đầu từ đầu `arrays` hoặc `slices` và tìm ra từng phần tử một.

Điều gì sẽ xảy ra nếu một loại bộ sưu tập mà mọi giá trị đều có `key` của nó. Bạn sẽ tìm thấy giá trị bạn muốn nhanh hơn. Và trong chương này, chúng tôi sẽ giới thiệu `maps`, thứ có thể làm điều trên.

`------`

### Chương 8: Đôi lúc bạn cần lưu trữ nhiều hơn một loại dữ liệu.

Chúng ta đã học về `slices`, thứ lưu trữ một danh sách giá trị. Sau đó, chúng ta đã học về maps, nơi ánh xạ danh sạch các khóa thành danh sách giá trị. Nhưng cả hai loại dữ liệu trên chỉ có thể giữ những giá trị có cũng một loại. Đôi khi, bạn cần phải nhóm các giá trị của một số loại lại với nhau. Hãy nghĩ đến địa chỉ gửi thư. nơi bạn kết hợp tên đường (strings) - mã số bưu điện (int). Hoặc là bản ghi về học sinh, nơi bạn kết hợp tên học sinh (strings) với điểm số trung bình (float). Bạn không thể kết hợp giá trị ở slice và maps được. Nhưng bạn có thể nếu bạn sử dụng một loại khác gọi là `struct`. Chúng ta sẽ học tất cả những thứ về `structs` trong chương này.

`------`

### Chương 9: Có nhiều thứ cần học về khai báo types.

Ở chương trước, chúng tôi đã cho bạn thấy cách mà khai báo một `struct` cơ bản. Điều mà chúng tôi không cho bạn thấy là bạn có thể sử dụng bất kì loại dữ liệu cơ bạn nào.

Và bạn có nhớ `methods` - một loại function đặc biệt được liên kết với các giá trị của một loại cụ thể. Chúng ta sẽ gọi đến một methods về giá trị khác nhau trong cuốn sách này. nhưng chúng tôi chưa chỉ cho bạn cách khai báo một methods của riêng bạn. Ở trong chương này, chúng ta sẽ làm tất cả điều đó. Nào bắt đầu thôi.

`------`

### Chương 10: Sai lầm xảy ra.

Thi thoảng, chương trình của chúng ta sẽ nhận những giá trị không hợp lệ từ phía người dùng, một tệp bạn đang đọc hoặc ở nơi khác. Ở chương này, bạn sẽ học cách đóng gói: cách bảo vệ các trường của loại cấu trúc của bạn khỏi dữ liệu không hợp lệ nào đó. Bằng cách đó, bạn sẽ biết dữ liệu trường của mình an toàn để làm việc.

Chúng tôi cũng sẽ chỉ cho bạn cách nhúng một loại dữ liệu khác trong `struct` của bạn. Nếu `struct` của bạn cần một phương thức khác đã tồn tại trong một loại khác, bạn không cần copy paste code của phương thức đó. Bạn có thể nhúng môt loại khác ở trong kiểu struct của bạn and sử dụng method của loại đã nhúng đó giống như chúng được xác định tên loại riêng của bạn.

`------`

### Chương 11: Đôi khi bạn không quan tâm đến loại giá trị cụ thể.

Bạn không quan tâm nó là cái gì. Bạn chỉ cần biết nó sẽ có thể làm một số điều. Bạn có thể gọi `Certain methods` trên đó. Bạn không cần quan tâm liệu bạn có bút hay bút chì, bạn chỉ cần một `Draw method`. Bạn không cần liệu bạn có Car hay Boat, chỉ cần một `Steer method`.

Đây là cách mà `Go interface` đạt được. Chúng cho phép bạn xác định các biến và tham số hàm sẽ giữ bất ký kiểu nào, miễn là kiễu đó xác định các phương thức nhất định.

`------`

### Chương 12: Mọi chương trình đều gặp lỗi. Bạn nên lập kế hoạch cho chúng.

Đôi khi việc xử lý một số lỗi có thể đơn giản như báo cáo và thoát khỏi chương trình. Nhưng một số lỗi khác có thể yêu cầu thêm hành động. Bạn có thể cần đóng files hoặc kết nối mạng hoặc nếu không thì xóa sạch, vì thế chương trình của bạn không để lại một mớ hỗn độn. Trong chương này, chúng tôi sẽ chỉ cho bạn làm sao để `defer` các hành động dọn dẹp để chúng diễn ra ngay cả khi có lỗi. Chúng tôi sẽ chỉ cho bạn làm sao để tạo ra một chương trình `panic` trong những tình huống thích hợp và làm thế nào để recover sau đó.

`------`

### Chương 13: Làm từng việc một lúc không phải lúc nào cũng là cách nhanh nhất để kết thúc một công việc.

Một vài vấn đề lớn có thể chia thành các nhiệm vụ nhỏ hơn. `Gorountines` để chương trình của bạn hoạt động các nhiệm vụ khác nhau cùng một lúc. `Goroutines` của bạn có thể phối hợp sử dụng chính `channels`, thứ có thể gửi data tới nơi khác và đồng bộ hóa vì thế `Goroutines` không đi trước người khác. Gorountines để bạn tận dụng tối đa vi xử lý đa nhân của máy tính. vì thế chương trình của banj chạy nhanh hơn nó có thể làm được.

`------`

### Chương 14: Bạn có chắc là phần mềm của bạn đang hoạt động một cách đúng đắn? Thật sự chứ?

Trước khi bạn gửi một phiên bản mới cho người dùng của bạn, bạn có lẽ thử hết các tính năng mới để đảm bảo nó hoạt động. Nhưng bạn có thử tính năng cũ và đảm bảo bạn không phá vỡ bất cứ thứ gì? Toàn bộ tính năng cũ? Nếu câu hỏi đó làm bạn lo lắng, chương trình của bạn cần `automated testing`. `Automated test` đảm bảo thành phần chương trình đảm bảo đúng đắn, ngay cả sau khi bạn thay đổi code của mình. Gói `Go's testing` and `go test tool` làm nó dễ dàng để viết `automated tests`, sử dụng kĩ năng bạn vừa học được.

`------`

### Chương 15: Bây giờ là thế kỉ 21. Người dùng muốn web apps.

Go cũng giúp bạn có mặt ở đó. Gói thư viện chuẩn của Go giúp bạn lưu trữ các ứng dụng web của riêng mình và làm cho chũng có thể truy cập được từ mọi trình duyệt web. Vì thế chúng ta sẽ dành hai chương cuối để chỉ bạn cách xây dựng một web apps.

Thứ đầu tiên của web app cần là khả năng phản hồi khi trình duyện gửi một yêu cầu. Ở chương này, chúng ta sẽ học cách sử dụng gói `net/http` để làm điều đó.

`------`

### Chương 16: Web apps của bạn cần trả về HTML, không phải plain text.

`Plain text` là tốt cho emails và bà đăng trên mạng xã hội. Nhưng trang của bạn cần một định dạng. Nó cần phần đầu và đoạn văn. Nó cần forms nơi mà người dùng có thể gửi data tớ app của bạn. Để làm bất cứ điều đó, bạn cần HTML code.

Và cuối cùng, bạn cần thêm data và HTML code. Đó là lý do tại sao Go cung cấp `htm/template`, một cách mạnh mẽ bao gồm data app của bạn trong HTML trả về. Templates là chìa khóa để xây dựng lớn hơn, tốt hơn web apps, and trong chương cuối, chúng tôi sẽ chỉ bạn cách sử dụng nó.
