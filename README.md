# BÀI LÀM: XÂY DỰNG PRIORITIZED PRODUCT BACKLOG BẰNG MoSCoW

## 1. Phân loại 12 hạng mục theo MoSCoW

Với vai trò Product Owner, tôi ưu tiên các chức năng giúp độc giả thực hiện được quy trình mượn sách giấy online và giúp thư viện quản lý sách. Do năng lực Release 1 chỉ khoảng 20 điểm, nhóm cần giới hạn Must để tập trung vào giá trị cốt lõi của MVP.

| STT | Hạng mục backlog                                       | Công sức | Nhóm MoSCoW | Lý do phân loại                                                                                                |
| --- | ------------------------------------------------------ | -------- | ----------- | -------------------------------------------------------------------------------------------------------------- |
| 1   | Đăng nhập/đăng ký tài khoản độc giả                    | M (2)    | Must        | Cần xác định danh tính độc giả để quản lý yêu cầu mượn sách và giới hạn số sách được mượn.                     |
| 2   | Tìm kiếm sách theo tên/tác giả                         | M (2)    | Must        | Là chức năng cốt lõi giúp độc giả tìm được sách cần mượn.                                                      |
| 3   | Mượn sách online (có giới hạn số sách mượn cùng lúc)   | L (3)    | Must        | Là nghiệp vụ chính của hệ thống, phụ thuộc vào tài khoản độc giả và dữ liệu sách.                              |
| 4   | Gia hạn mượn sách online                               | S (1)    | Could       | Có thể xử lý gia hạn trực tiếp tại quầy trong giai đoạn đầu mà không ảnh hưởng đến chức năng mượn sách cơ bản. |
| 5   | Đặt trước sách khi hết (kèm thông báo khi sách có sẵn) | M (2)    | Should      | Tăng khả năng phục vụ độc giả khi sách hết, nhưng có thể triển khai sau khi quy trình mượn sách đã ổn định.    |
| 6   | Đánh giá & bình luận sách sau khi đọc                  | M (2)    | Won't       | Không trực tiếp phục vụ nghiệp vụ mượn sách của MVP và cần thêm cơ chế quản lý nội dung người dùng.            |
| 7   | Gợi ý sách theo sở thích cá nhân                       | L (3)    | Won't       | Là chức năng nâng cao, tốn công sức và cần dữ liệu sở thích hoặc lịch sử để tạo gợi ý hữu ích.                 |
| 8   | Thông báo email khi sắp đến hạn trả sách               | S (1)    | Should      | Giúp hạn chế trả sách muộn, nhưng giai đoạn đầu có thể nhắc độc giả bằng cách khác.                            |
| 9   | Xem lịch sử mượn sách của bản thân                     | S (1)    | Could       | Hữu ích cho độc giả nhưng không bắt buộc để hoàn thành giao dịch mượn sách cơ bản.                             |
| 10  | Thủ thư quản lý kho sách (thêm/sửa/xóa sách)           | L (3)    | Must        | Cần dữ liệu sách và số lượng sách được cập nhật để chức năng tìm kiếm, mượn sách hoạt động đúng.               |
| 11  | Chat trực tiếp với thủ thư                             | L (3)    | Won't       | Có thể thay bằng liên hệ trực tiếp hoặc điện thoại, tránh phát sinh chi phí xây dựng hệ thống chat.            |
| 12  | Tích hợp đăng nhập bằng Google/Facebook                | M (2)    | Could       | Có thể dùng đăng ký và đăng nhập bằng tài khoản nội bộ, nên tích hợp mạng xã hội chưa phải yêu cầu thiết yếu.  |

Lưu ý: Đây là phương án phân loại đề xuất. MoSCoW không phụ thuộc hoàn toàn vào kích thước S/M/L; một hạng mục tốn nhiều công sức vẫn có thể là Must nếu thiếu nó khiến MVP không thể vận hành.

## 2. Tính tổng công sức nhóm Must

Các hạng mục Must gồm:

| Hạng mục                       | Công sức |
| ------------------------------ | -------- |
| 1. Đăng nhập/đăng ký tài khoản | 2        |
| 2. Tìm kiếm sách               | 2        |
| 3. Mượn sách online            | 3        |
| 10. Thủ thư quản lý kho sách   | 3        |
| Tổng cộng                      | 10 điểm  |

Năng lực Release 1 là khoảng 20 điểm.

Tỷ lệ Must=1020×100%=50%\text{Tỷ lệ Must}=\frac{10}{20}\times100\%=50\%Tỷ lệ Must=2010×100%=50%

Kết luận: 10 điểm, tương đương 50% năng lực Release 1. Tổng này không vượt ngưỡng khoảng 60% (12 điểm), nhưng thấp hơn mục tiêu tham khảo 12 điểm. Điều này tạo dư địa cho các hạng mục Should và những phát sinh trong quá trình phát triển.

## 3. Prioritized Product Backlog có thứ tự từ 1 đến 12

Backlog được sắp xếp theo thứ tự ưu tiên duy nhất. Các mục Must đứng trước Should, tiếp theo là Could và Won't. Trong từng nhóm, thứ tự được cân nhắc theo phụ thuộc kỹ thuật và giá trị nghiệp vụ.

| Thứ tự | ID | Hạng mục                                      | Nhóm   | Điểm | Giải thích thứ tự                                                              |
| ------ | -- | --------------------------------------------- | ------ | ---- | ------------------------------------------------------------------------------ |
| 1      | 1  | Đăng nhập/đăng ký tài khoản độc giả           | Must   | 2    | Tạo danh tính độc giả trước khi thực hiện giao dịch mượn.                      |
| 2      | 10 | Thủ thư quản lý kho sách                      | Must   | 3    | Cung cấp dữ liệu sách và số lượng hiện có cho các chức năng tiếp theo.         |
| 3      | 2  | Tìm kiếm sách theo tên/tác giả                | Must   | 2    | Giúp độc giả tìm sách dựa trên dữ liệu kho sách đã có.                         |
| 4      | 3  | Mượn sách online, giới hạn số sách            | Must   | 3    | Hoàn thiện nghiệp vụ cốt lõi sau khi có tài khoản và dữ liệu sách.             |
| 5      | 5  | Đặt trước sách khi hết, thông báo khi có sách | Should | 2    | Mở rộng quy trình mượn sách, cần dữ liệu tồn kho và cơ chế xử lý yêu cầu mượn. |
| 6      | 8  | Email nhắc sắp đến hạn trả sách               | Should | 1    | Tăng hiệu quả quản lý thời hạn sau khi quy trình mượn đã hoạt động.            |
| 7      | 9  | Xem lịch sử mượn sách                         | Could  | 1    | Tận dụng dữ liệu giao dịch đã lưu, cải thiện trải nghiệm độc giả.              |
| 8      | 4  | Gia hạn mượn sách online                      | Could  | 1    | Mở rộng nghiệp vụ hiện có, có thể xử lý thủ công trong MVP.                    |
| 9      | 12 | Đăng nhập bằng Google/Facebook                | Could  | 2    | Cải thiện sự tiện lợi nhưng không thay thế nhu cầu có tài khoản độc giả.       |
| 10     | 6  | Đánh giá và bình luận sách                    | Won't  | 2    | Chưa cần thiết cho quy trình mượn sách; để lại cho bản phát hành sau.          |
| 11     | 11 | Chat trực tiếp với thủ thư                    | Won't  | 3    | Có thể dùng kênh liên hệ hiện có thay thế.                                     |
| 12     | 7  | Gợi ý sách theo sở thích cá nhân              | Won't  | 3    | Chức năng nâng cao, cần thêm công sức và dữ liệu để triển khai hiệu quả.       |

### Kiểm tra tổng điểm theo nhóm

| Nhóm   | Số hạng mục | Tổng điểm |
| ------ | ----------- | --------- |
| Must   | 4           | 10        |
| Should | 2           | 3         |
| Could  | 3           | 4         |
| Won't  | 3           | 8         |
| Tổng   | 12          | 25        |

Như vậy, toàn bộ 12 hạng mục đều được giữ lại trong Product Backlog và tổng công sức là 25 điểm, đúng với dữ liệu đề bài. Nhóm có thể thực hiện toàn bộ Must (10 điểm), sau đó ưu tiên Should (3 điểm). Nếu năng lực thực tế còn khoảng 7 điểm, nhóm có thể xem xét một phần Could sau khi đánh giá rủi ro và tiến độ.

## 4. Tự phản biện quyết định ưu tiên

Có thể có những ý kiến khác nhau về một số hạng mục:

* Mục 5 – Đặt trước sách: Một người có thể xếp vào Must vì đặt trước là cách quan trọng để phục vụ độc giả khi sách đã được mượn hết. Tuy nhiên, tôi chọn Should vì MVP vẫn có thể vận hành với các sách còn sẵn; đặt trước là chức năng mở rộng sau khi luồng mượn cơ bản hoạt động ổn định.

* Mục 12 – Đăng nhập Google/Facebook: Một người có thể xếp vào Should vì đăng nhập nhanh giúp giảm thao tác và cải thiện trải nghiệm. Tôi xếp Could vì tài khoản nội bộ đã đáp ứng nhu cầu xác thực, nên tích hợp bên thứ ba chưa cấp thiết.

* Mục 6 – Đánh giá và bình luận sách: Có thể xếp vào Could vì tính năng này giúp tăng tương tác và cung cấp thông tin tham khảo. Tôi xếp Won't để tập trung nguồn lực vào nghiệp vụ thư viện trong Release 1.

* Mục 7 – Gợi ý sách: Có thể xếp vào Could nếu thư viện muốn tăng mức độ khám phá sách ngay từ đầu. Tôi xếp Won't vì đây là chức năng nâng cao, cần thêm dữ liệu và công sức, trong khi mục tiêu MVP là hoàn thành quy trình mượn sách giấy online.

## 5. Kết luận

Phương án trên đáp ứng các ràng buộc của đề bài: chỉ có 4 hạng mục Must, tổng Must là 10 điểm và không vượt ngưỡng 12 điểm; cả 12 hạng mục đều được phân loại đúng một nhóm và có thứ tự từ 1 đến 12.

Về nguyên tắc, Product Owner chịu trách nhiệm sắp xếp Product Backlog theo giá trị, rủi ro, phụ thuộc và thông tin mới. Thứ tự này cần được xem xét lại khi có dữ liệu thực tế từ độc giả, thay đổi năng lực nhóm hoặc điều chỉnh mục tiêu Release 1.
