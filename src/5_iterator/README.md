# Iterator Pattern là gì?

* Iterator Pattern là một trong những Pattern thuộc nhóm nhóm hành vi (Behavior Pattern)
* Nó được sử dụng để “Cung cấp một cách thức truy cập tuần tự tới các phần tử của một 
đối tượng tổng hợp, mà không cần phải tạo dựng riêng các phương pháp truy cập cho đối tượng tổng hợp này”.

* Nói cách khác, một Iterator được thiết kế cho phép xử lý nhiều loại tập hợp khác nhau bằng cách truy cập những phần tử của tập hợp với cùng một phương pháp,cùng một cách thức định sẵn, mà không cần phải hiểu rõ về những chi tiết bên trong của những tập hợp này.

* 1 Template method thường sẽ có interface class và Concrete Class 

# Lợi ích 
* Đảm bảo nguyên tắc Single responsibility principle (SRP) : chúng ta có thể tách phần cài đặt các phương thức của tập hợp và phần duyệt qua các phần tử (iterator) theo từng class riêng lẻ.
* Đảm bảo nguyên tắc Open/Closed Principle (OCP) : chúng ta có thể implement các loại collection mới và iterator mới, sau đó chuyển chúng vào code hiện có mà không vi phạm bất cứ nguyên tắc gì.

# Dùng khi nào
* Cần truy cập nội dung của đối tượng trong tập hợp mà không cần biết nội dung cài đặt bên trong nó.
* Hỗ trợ truy xuất nhiều loại tập hợp khác nhau.
* Cung cấp một interface duy nhất để duyệt qua các phần tử của một tập hợp.