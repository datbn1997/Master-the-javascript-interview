[nguồn](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
# Cuộc phỏng vấn Master The JavaScript: functional programming là gì ?
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

Pure functions có rất nhiều thuộc tính quan trọng trong functional programming, bao gồm **referential transparency**(bạn có thể thay thế 1 lời gọi hàm với kết quả trả về không làm thay đổi chương trình). Đọc \"What is a Pure Function?\" để biết chi tiết hơn 




