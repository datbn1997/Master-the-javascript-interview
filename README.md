[nguồn](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
# Master The JavaScript Interview: functional programming là gì ?
> *"Cuộc phỏng vấn Master The JavaScript" là 1 series của những bài viết được viết ra để chuẩn bị cho những câu hỏi thường gặp, rất có thể họ sẽ gặp khi ứng tuyển vào vị trí từ level trung bình đến senior của JavaScript. Những câu hỏi mà tôi thường xuyên sử dụng trong một cuộc phỏng vấn*.

**Functional programming** đã trở thành 1 chủ đề hot của JavaScript trên toàn thế giới. Trong 1 vài năm trước, một số lập trình viên JavaScript cũng đã biết được functional programming là gì. Nhưng mỗi ứng dụng có codebase lớn mà tôi đã gặp trong suốt 3 năm nó sẽ nặng nề khi bạn sử dụng functional programming.

**Functional programming**(thường được viết tắt là **FP**) là một tiến trình xây dựng phần mềm với các pure function, tránh **shared state**, **mutable data** và **side-effects**. Functional programming có tính **declarative** thay vì bắt buộc, và những trạng thái của ứng dụng sẽ thông qua các hàm pure functional. Trái với lập trình hướng đối tượng, ở đó các trạng thái của ứng dụng thường xuyên được chia sẻ và colocated với phương thức của đối tượng.

**Funcitional programming** là 1 mô hình lập trình, điều đó nghĩa là đây là 1 cách suy nghĩ về việc xây dựng phần mềm dựa trên những điều cơ bản, những quy tắc đã được định nghĩa (đã được liệt kê ở trên). Một ví dụ khác của mô hình lập trình,nó bao gồm lập trình hướng đối tượng và lập trình hướng thủ tục.

Code của lập trình hướng chức năng có xu hướng ngắn gọn hơn, dễ đoán và dễ dàng cho việc test hơn là code lập trình hướng đối tượng. Nhưng nếu bạn cảm thấy không quen với nó, và những pattern phổ biến liên kết với nó, code theo hướng functional có thể nhiều hơn và những từ ngữ, văn chương có thể khó hiểu đối với người mới học.

Nếu bạn tra cứu google với từ khóa functional programming thì bạn sẽ nhanh chóng bị cản trở bởi khó khăn, nó thật đáng sợ đối với những người mới bắt đầu. Một lời nói dối trầm trọng nếu nói nó có cách học "curve". Nếu bạn đã học JavaScript trong 1 thời gian, một cơ hội tốt để cho bạn sử dụng những khái niệm hay tiện ích trong phần mềm của bạn.
> *Đừng để những từ mới làm cho bạn sợ hãi. Nó có vẻ dễ hơn bạn tưởng*

Phần khó nhất đó là những từ ngữ không quen luôn xuất hiện quanh đầu bạn. Có nhiều ý tưởng đơn giản để định nghĩa những từ bên trên. Bạn cần phải hiểu tất cả những định nghĩa từ bên trên trước khi bắt đầu học functional programming.

* Pure functions
* Function composition
* Avoid shared state
* Avoid mutable state

Nói cách khác, nếu bạn muốn biết functional programming là gì trong thực tế, bạn phải hiểu những cốt lõi khái niệm. 

**Pure function** là một hàm khi:

* gửi cùng 1 đầu vào và luôn luôn trả về 1 đầu ra.
* không bị ảnh hưởng ở bên ngoài

Pure functions có rất nhiều thuộc tính quan trọng trong functional programming, bao gồm **referential transparency**(bạn có thể thay thế 1 lời gọi hàm với kết quả trả về không làm thay đổi chương trình). Đọc [\"What is a Pure Function?\"](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976) để biết chi tiết hơn.

**function composition** là một tiến trình kết hợp của 2 hay nhiều function để tạo ra một hàm tính toán mới. Ví dụ Thành phần `f . g` (dấu chấm nghĩa là "kết hợp với") nó tương đương với `f(g(x))` trong JavaScript. Sự hiểu biết về function composition rất quan trọng để tiến tới hiểu được một phần mềm được xây dựng và sử dụng functional programming thế nào. Đọc [\"What is Function Composition?\"](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-function-composition-20dfb109a1a0) để hiểu rõ hơn.

### **Shared State**
**Shared State** là tổng hợp rất nhiều biến, đối tượng hoặc bộ nhớ trống điều đó tồn tại trong phạm vi nào đó được chia sẻ, hay với thuộc tính của đối tượng nào đó được truyền vào trong phạm vi. Phạm vi chia sẻ bao gồm phạm vi toàn cục, pham vi cục bộ. Thông thường trong lập trình hướng đối tượng, các đối tượng được chia sẻ trong phạm vi bằng cách thêm các thuộc tính vào đối tượng khác.

Ví dụ, Một trò chơi máy tính phải có đối tượng chính trong game, với nhân vật và các items trong game lưu trữ các thuộc tính của họ bởi chính đối tượng đó. Functional programming tránh shared state-thay vì dựa vào cấu trúc dữ liệu không thay đổi, các phép tính thuần túy để lấy được dữ liệu mới từ các dữ liệu có sẵn. Để chi tiết hơn về cách mà các phần mềm hướng chức năng có thể xử lý trạng thái của ứng dụng bạn xem [\"10 tips for better Relux Architeture?\"](https://medium.com/javascript-scene/10-tips-for-better-redux-architecture-69250425af44)

Vấn đề của shared state chính là bạn phải hiểu được những ảnh hưởng của hàm,bạn phải biết lịch sử toàn thể của các biến mà bạn đã chia sẻ khi sử dụng hàm hoặc những ảnh hưởng mà nó gây ra.

Tưởng tượng bạn có một đối tượng user và bạn cần save. Hàm `saveUser()` sẽ tạo một request tới API trên server. Trong khi nó đang thực hiện, người dùng thay đổi thông tin ảnh cá nhân với `updateAvatar()` và gây ra bởi một request `saveUser()` khác. Khi được lưu, Server sẽ trả về đối tượng người dùng mà nên thay thế bất cứ thứ gì trong bộ nhớ để có thể đồng bộ với những gì xảy ra trên server hoặc những reponse của những lời gọi API khác.

Thật không may, reponse thứ 2 đã được nhận trước reponse đầu tiên, vậy khi trong lần reponse thứ 1(đã bị lỗi thời) trả về, ảnh mới trong profile đã bị xóa trong bộ nhớ và đã bị thay thế bởi 1 số cũ. Đây là ví dụ chạy điều kiện-1 lỗi phổ biến liên quan đến shared state

Những lỗi phổ biến với shared state đó là thay đổi trật tự của các hàm được gọi có thể gây ra thất bại liên tiếp bởi vì những hàm nào có những hành động shared state đều trong phụ thuộc vào thời gian.

Khi bạn tránh shared state, thời gian và trật tự của hàm gọi sẽ không bị thay đổi kết quả của việc gọi hàm. Với pure function, gửi cùng 1 đầu vào, bạn sẽ luôn nhần cùng 1 đầu ra. Điều này làm cho các lời gọi hàm hoàn toàn độc lập với các lời gọi hàm khác, hoàn toàn có thể đơn giản thay đổi và tái cấu trúc. Sự thay đổi trong 1 hàm, hoặc thời gian của lời gọi hàm không ảnh hướng và phá vỡ các phần của chương trình.

Trong ví dụ trên, chúng tôi sử dụng `object.assign()` và truyền trong 1 đối tượng rỗng như là 1 tham số đầu tiên để sao chép thuộc tính `x` thay vì biến đổi bên trong nó. Trong trường hợp này, nó tương đương với việc bạn tạo ra 1 đối tượng mới từ SCratch không có `object.assign()`. Nhưng đây là pattern phổ biến trong JavaScript để tạo bản sao trạng thại hiện tại thay vì sử dụng thay thế biến đổi, mà chúng tôi chứng minh ở ví dụ trên. 

Nếu bạn để ý trong lệnh `consonle.log()` ở ví dụ này, bạn cần để ý 1 vài thứ được đề cập đến: function composition. Nhắc lại, function composition như là `f(g(x))`. Trong trường hợp này chúng ta sẽ thay thế `f()` và `g()` với `x1()` và `x2()` sẽ cho ra `x1 . x2 `.

Dĩ nhiên, Nếu bạn muốn thay đổi thứ tự trong thành phần của nó đầu ra sẽ thay đổi. Thứ tự của phép tính vẫn là vấn đề. `f(g(x))` không phải luôn luôn bằng `g(f(x))`, nhưng vấn đề gì xảy ra ra nữa không, chuyển gì xảy ra ở các biến ở ngoài hàm - và đây là vấn đề lớn. Với các hàm impure. Nó không thể hiểu toàn bộ 1 hàm làm những gì trừ khi bạn biết toàn bộ lịch sử của toàn bộ biến mà hàm đã sử dụng và những ảnh hưởng của nó.

Xóa hàm phụ thuộc vào thời gian. Và bạn loại trừ toàn thể lớp có tiềm năng chứ bug.

## **Immutability**









