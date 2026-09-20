Phần 1 – Phân tích vai trò UI State

Tại sao cần thiết kế nhiều trạng thái tĩnh trước khi làm Prototype?

Nút “Thanh toán” không chỉ có một trạng thái. Trước khi nối Prototype, cần thiết kế rõ các trạng thái để người dùng, Tester và lập trình viên hiểu nút sẽ hiển thị như thế nào trong từng tình huống.

Ba trạng thái cần có:

Disabled: khi khách hàng chưa nhập đủ thông tin thanh toán.
Default: khi thông tin hợp lệ và nút sẵn sàng được bấm.
Loading: khi hệ thống đang xử lý giao dịch.

Việc thiết kế trước các UI State giúp Prototype rõ ràng hơn và giúp lập trình viên triển khai đúng giao diện.

Nếu nút luôn sáng màu thì gây nhầm lẫn gì?

Nếu nút “Thanh toán” luôn hiển thị ở trạng thái có thể bấm dù form còn trống, người dùng có thể nghĩ rằng họ đã đủ điều kiện thanh toán. Tester cũng khó xác định khi nào nút được phép hoạt động và khi nào phải bị vô hiệu hóa.

Điều này khiến Prototype không phản ánh đúng quy tắc nghiệp vụ.

Phần 2 – Thiết kế trên Figma

Chỉ cần tạo 3 phiên bản tĩnh của nút “Thanh toán”:

Trạng thái	Thiết kế
Disabled	Nút xám nhạt, chữ “Thanh toán” màu xám, thể hiện chưa thể bấm
Default	Nút xám đậm, chữ “Thanh toán” rõ ràng, thể hiện sẵn sàng bấm
Loading	Nút xám đậm, có biểu tượng vòng tròn tải và chữ “Đang xử lý...”

Ví dụ bố cục:

[ Thanh toán ] — Disabled, màu nhạt

[ Thanh toán ] — Default, màu đậm

[ ◌ Đang xử lý... ] — Loading

Không cần nối dây Prototype, không cần tạo tương tác Hover hoặc Click. Chỉ đặt 3 trạng thái cạnh nhau trên cùng một Frame để tạo một UI Kit nhỏ.
Link figma: https://www.figma.com/design/TETLritCIkBekQ6PUBN3rA/Untitled?node-id=0-1&p=f&t=5PvDchOXdIezrf4W-0