## Chương 1: Bắt đầu thôi: Cú pháp cơ bản

Bạn đã thực sự tăng áp cho ứng dụng của mình chưa? Bạn có muốn một ngôn ngữ đơn giản, biên dịch nhanh? Chạy nhanh? Dễ dàng phân phối tới người sử dụng. Sau đó bạn đã sẵn sàng học Go!

Go là một ngôn ngữ lập trình tập trung vào sự đơn giản và tốc độ. Nó đơn giản hơn những ngôn ngữ khác, vì thế dễ dàng để học. Và nó cho phép bạn khai thác sức mạnh vi xử lý máy tính nhiều lõi ngày nay, vì thế chương trình chạy nhanh hơn. Chương này sẽ cho bạn thấy tính năng của Go làm cho cuộc sống của bạn như là một developer dễ dạng hơn, và làm cho người dùng của bạn hạnh phúc hơn.

**Sẵn sàng, Bắt đầu!**

Quay trở lại năm 2007, công cụ tìm kiếm của Google có vấn đề. Nó buộc phải bảo trì chương trình với hàng tỉ dòng code. trước khi họ có thể thử sự thay đổi mới, họ buộc phải biên dịch code thành một mã dạng có thể chạy được, một quy trình vào thời điểm đó mất hơn 1h. Không cần phải nói, điều này không hề tốt cho năng suất của nhà phát triển.

Vì thế các kĩ sư của Google `Robert Gresemer`, `Rob Pike` và `Ken Thompson` phác thảo mục tiêu cho một ngôn ngữ mới:

- Biên dịch nhanh

- Code bớt rườm rà hơn

- Tự động giải phóng bộ nhớ không sử dụng

- Phần mềm dễ viết thực hiện nhiều thao tác đồng thời

- Hỗ trợ tốt cho những vi xử lý nhiều nhân.

Sau một vài năm làm việc, Google tạo ra Go: một ngôn ngữ viết code nhanh và tạo ra các chương trình nhanh chóng biên dịch và chạy. Dự án chuyển sang giấy phép mã nguồn ở vào năm 2009. Và giờ miễn phí cho mọi người sử dụng. Và bạn nên sử dụng nó! Go. Go nhanh chóng trở nên phổ biến nhờ sự đơn giản và sức mạnh của nó.

Nếu bạn đang viết command-line tool, Go có thể sản xuất một file thực thi cho Windows, macOS và Linux, tất cả từ cùng một mã nguồn. Nếu bạn đang viết web server, nó có thể xử lý nhiều user kết nối tại một thời điểm. Và bất kể bạn đang viết gì, nó sẽ giúp bạn đảm bảo code của bạn dễ bảo trì và thêm vào.

**Sẵn sàng để học nhiều hơn? Bắt đầu thôi.**

**The Go Playground**

Cách tốt nhất để thử Go là vào ghé thăm [https://play.golang.org](https://play.golang.org/) ở trên trình duyệt của bạn. Ở đó, team Go đã cài đặt sẵn một trình soạn thảo đơn giản nơi bạn có thể nhập Go code và chạy nó ở trên server của họ. Kết quả sẽ hiện thị ngay trên trình duyệt của bạn. Dĩ nhiên nó chỉ hoạt động nếu mà bạn có kết nối mạng ổn định. Nếu không, hãy học cách tải và chạy Go biên dịch trên máy tính của bạn. Sau đó chạy chương trình mẫu sử dụng trình biên dịch thay thế.

Hãy thử nó ngay bây giờ.

1. Mở [https://play.golang.org](https://play.golang.org/) ở trình duyệt của bạn. Đừng lo lắng nếu bạn không khớp với ảnh chụp màn hình, điều đó có nghĩa họ đã cải thiện trang web kể từ khi cuốn sách này được in.

2. Xóa bất cứ dòng code nào ở nơi chỉnh sửa, và nhập vào dòng sau thay thế:

```
package main

import "fmt"

func main() {

    fmt.Println("Hello, Go!")

}
//Đừng lo lắng gì cả, chúng tôi sẽ giải thích trong tất cả.
```

3. Nhấn vào nút `Format`, sẽ tự động định dạng lại code theo `Go conventions`.
4. Nhấn nút `Run`.

Bạn nên nhìn thấy `Hello, Go!` hiện thị ở dưới màn hình. Chúc mừng, bạn vừa chạy chương trình Go đầu tiên.
Ở trang tiếp theo, chúng tôi sẽ giải thích chúng ta vừa làm gì...

### Tất cả nó có ý nghĩa gì?

Bạn vừa chạy chương trình Go đầu tiên! Bây giờ, nhìn vào code và tìm ra những gì nó thực sự có nghĩa...

Mọi file Go bắt đầu với mệnh đề `package`. Một `package` là một tập hợp code, tất cả đều làm điều tương tự, như định dạng một chuỗi hoặc là vẽ một hình ảnh. Mệnh đề `package` cho biết tên của gói nơi file code sẽ trở thành một phần. Trong trường hợp này, chúng tôi sử dụng gói đặc biệt `main`, thứ bắt buộc nếu mã này sẽ được chạy trực tiếp(thường là từ `termnial`).
Tiếp đến, Go file luôn luôn có một hoặc nhiều câu lệnh `import`. Mỗi file cần `import` từ một `package`trước khi code có thể được sử dụng từ các gói khác. Tải tất cả Go code ở trong máy tính của bạn trong một lần sẽ dẫn đến một chương trình lớn, chương trình chậm, vì thế thay vào đó bạn chỉ nên xác định các gọi bạn cần bằng cách nhập chúng.
Phần cuối cùng của mọi Go file là code thực sự, cái mà thường được chia thành một hay nhiều `functions`. Một `functions` là một tập hợp một hoặc nhiều dòng code, bạn có thể `call(run)` từ những nơi khác ở trong chương trình của bạn. Khi mà chương trình Go chạy, nó tìm kiếm một function tên là `main` và chạy nó đầu tiên, đó là lý do tại sao chúng tôi đặt tên nó là `main`.


## Bố cục file Go điển hỉnh
Bạn sẽ nhanh chóng làm quen với việc 3 phần như này, theo thứ tự này, mọi file Go bạn làm với:
1. Mệnh đề ``package``
2. Cú pháp ``import``
3. Code

Câu nói ``một nơi cho mọi thứ, và mọi thứ ở đúng vị trí của nó``. Go là một ngôn ngữ nhất quán. Đây là một điều tốt: bạn thường xuyên tìm kiếm,  bạn chỉ cần tìm một đoạn mã nhất định trong dự án của mình mà không cần phải suy nghĩ về nó.

## Một vài chú ý
1. Bạn có thể sử dụng dấu chấm phẩy ở cuối dòng code, nhưng điều đó là không cần thiết.
Nó sẽ được lược bỏ nếu bạn sử dụng ``fmt``
2. ``Go convention`` đến từ ``fmt package``

## Hàm được gọi như thế nào?
Ví dụ của chúng ta bao gồm một function từ ``fmt package``. Để gọi một function, hãy lấy tên function đó (``Println`` trong trường hợp này), và một cặp dấu ngoặc đơn.
Giống như nhiều function, ``Println`` có thể nhận một hoặc nhiều ``arguments``: giá trị bạn muốn function làm việc với.
``Println`` có thể được gọi mà không cần ``arguments``, hoặc bạn có thể cung cấp một số ``arguments``. Khi chúng ta xem xét các chức năng khác sau, tuy nhiên, bạn sẽ tìm kiếm hầu hết một tham số cụ thể. Nếu bạn cung cấp nhiều hơm, bạn sẽ nhận được thông báo lỗi số lượng tham số mong chờ và bạn sẽ sửa code của bạn.

## The Println function
Sử dụng ``Println function`` khi bạn muốn nhìn thấy chương trình của bạn đang làm. Bất cứ tham số bạn truyền vào nó sẽ được in ra(hiện thị) ở trên ``terminal`` của bạn, mỗi tham số được ngăn cách bởi một dòng.

Sau khi in hết những tham số, ``Println`` sẽ bỏ qua một dòng trên ``terminal``. (Đó là lý do tại sao nó có ``ln`` ở trong tên)

## Sử dụng function từ một package khác.
Code trong chương trình đầu tiên của chúng ta là một phần của gói ``main``, nhưng ``Println`` function ở trong gói ``fmt``. Để có thể sử dụng ``Println``, đầu tiên chúng ta phải ``import`` gói chứa nó.

Một khi chúng ta ``import`` gói, chúng ta có thể truy cập bất cứ function nào. Sử dụng cú phát `` name package + . + name function`` để sử dụng function mà chúng ta muốn.
```
Ex: fmt.Println()
```
Code mẫu sẽ gọi hàm từ hai gói khác. Bởi vì chúng ta muốn ``import`` nhiều gói, chúng ta chuyển sang một định dạng thay thế cho cú pháp ``import``, bạn có thể liệt kê danh sách gói bên trong ngoặc đơn, mỗi gói một dòng
```
package main
import (
    "math"
    "fmt"
    "strings"
)
function main() {
    math.Floor(2.75)
    strings.Title("Head first Go")
}
```
Chúng ta vừa ``import`` 2 gói là ``math`` và ``strings``, chúng ta có thể truy cập hàm ``Floor`` với cú pháp ``math.Floor`` và hàm ``Title`` với ``strings.Title``.