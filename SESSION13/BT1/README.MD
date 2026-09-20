# BÁO CÁO SỬA LỖI GIAO DIỆN FORM ĐĂNG KÝ RIKKEISHOP

## 1. Phân tích lỗi giao diện

| Nội dung                   | Phân tích                                                                                                                                                                                    |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Hiện trạng lỗi             | Trường **Giới tính** đang sử dụng **Checkbox** cho hai lựa chọn Nam và Nữ. Checkbox cho phép chọn nhiều giá trị cùng lúc nên người dùng có thể chọn cả Nam và Nữ.                            |
| Nguyên tắc UI bị vi phạm   | Vi phạm **Clarity** vì cách lựa chọn không rõ ràng với yêu cầu chỉ được chọn một giá trị. Đồng thời vi phạm **Affordance** vì Checkbox thể hiện khả năng chọn nhiều lựa chọn độc lập.        |
| Thành phần UI cần thay thế | Thay Checkbox bằng **Radio Button**.                                                                                                                                                         |
| Lý do                      | Radio Button được sử dụng khi người dùng chỉ được chọn **một giá trị duy nhất trong một nhóm lựa chọn**.                                                                                     |
| Xử lý dữ liệu              | Hai Radio Button Nam và Nữ phải thuộc cùng một nhóm để khi chọn Nam thì Nữ tự bỏ chọn và ngược lại. Có thể đặt một lựa chọn mặc định hoặc yêu cầu người dùng bắt buộc chọn trước khi Submit. |

## 2. Thiết kế Wireframe sau khi sửa

Trường Giới tính được sửa thành:

**Giới tính**

○ Nam
○ Nữ

Hai lựa chọn sử dụng **Radio Button** và nằm trong cùng một nhóm.

Ví dụ khi người dùng chọn Nam:

◉ Nam
○ Nữ

Khi người dùng chuyển sang chọn Nữ:

○ Nam
◉ Nữ

## 3. Kết luận

Việc thay **Checkbox bằng Radio Button** giúp giao diện phù hợp với quy tắc nghiệp vụ mỗi người dùng chỉ được chọn một giới tính. Thiết kế mới giúp tránh dữ liệu sai như chọn đồng thời cả Nam và Nữ, đồng thời làm Form đăng ký rõ ràng và dễ sử dụng hơn.
Link figma https://www.figma.com/design/gQBqLBLjAd5w3YIlAYeBba/RikkeiShop---S%25E1%25BB%25ADa-l%25E1%25BB%2597i-tr%25C6%25B0%25E1%25BB%259Dng-Gi%25E1%25BB%259Bi-t%25C3%25ADnh?node-id=0-1&p=f&t=Jj3qwQNBDS8r1ydo-0