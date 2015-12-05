4. Thiết kế giao diện người dùng
==========

Thiết kế giao diện người dùng là một phần quan trọng quá trình thiết kế phần mềm. Thiết kế giao diện và xử lý tương tác với người sử dụng là một yếu tố quan trọng trong việc sử dụng phần mềm. Người thiết kế phải làm sao để phù hợp với kĩ năng, kinh nghiệm và mong đợi từ phía người sử dụng phần mềm.


4.1: Nguyên tắc cơ bản trong thiết kế giao diện
-----------

- **Dễ học**: Phần mềm cần phải dễ học cách sử dụng, do đó người dùng có thể nhanh chóng bắt đầu làm việc sử dụng phần mềm đó
- **Quen thuộc với người sử dụng**: Giao diện nên dùng các thuật ngữ và khái niệm rút ra từ kinh nghiệm của những người sẽ dùng hệ thống nhiều nhất
- **Tính nhất quán**: giao diện cần nhất quán sao cho các thao tác gần giống nhau có thể được kích hoạt theo cùng kiểu.
- **Ngạc nhiên tối thiểu**: Người dùng không bao giờ bị bất ngờ về hành vi của hệ thống
- **Khôi phục được**: Giao diện nên có các cơ chế cho phép người dùng khôi phục lại tình trạng hoạt động bình thường sau khi gặp lỗi
- **Hướng dẫn người dùng**: Giao diện nên có phản hồi có nghĩa khi xảy ra lỗi và cung cấp các tiện ích trợ giúp theo ngữ cảnh
- **Người dùng đa dạng**: Giao diện nên cung cấp các tiện ích tương tác thích hợp cho các loại người dùng hệ thống khác nhau

4.2: Vấn đề trong thiết kế giao diện
-----------

Hai vấn đề cần xem xét:

- *Người dùng cung cấp thông tin cho hệ thống bằng cách nào?*
- *Hệ thống nên trình bày thông tin (output) cho người dùng như thế nào?*

4.3: Các kiểu tương tác
----------

Các kiểu tương tác phổ biến:

- **Thao tác trực tiếp** – Direct manipulation
- **Chọn lựa bằng menu** – Menu selection
- **Điền form** – Form fill-in
- **Dòng lệnh** – Command language
- **Ngôn ngữ tự nhiên** – Natural language


Kiểu tương tác | Ưu điểm chính | Nhược điểm chính | Ví dụ
-------------- | ------------- | ---------------- | -----
Thao tác trực tiếp | Tương tác trực quan, nhanh chóng và dễ hiểu | Có thể khó cài đặt. Chỉ thích hợp khi có ẩn dụ hình ảnh cho các tác vụ và đối tượng | Trò chơi điện tử và các ứng dụng có drag & drop
Chọn lựa bằng menu | Tránh lỗi cho người dùng, không phải làm nhiều thao tác | Chậm chạp với người sử dụng có kinh nghiệm. Có thể phức tạp nếu có nhiều lựa chọn menu | Đa số các hệ thống thông dụng
Điền form | Nhập dữ liệu đơn giản, dễ học, có thể kiểm tra được | Tốn không gian hiển thị, rắc rối khi lựa chọn của người dùng không khớp với kiểu dữ liệu của form | Đăng kí thông tin cá nhân, khai thuế
Dòng lệnh | Mạnh và linh động | Khó học, xử lý lỗi kém | Terminal, Autocad
Ngôn ngữ tự nhiên | Đáp ứng được người dùng không chuyên, dễ mở rộng | Cần gõ nhiều, các hệ thống hiểu ngôn ngữ tự nhiên không đáng tin cậy | Trợ lý ảo

4.4: Biểu diễn thông tin
---------------

Thông tin có thể được trình bày trực tiếp (ví dụ text trong một trình soạn thảo) hoặc được biến đổi thành một dạng biểu diễn khác (ví dụ dạng đồ họa)

Model-View-Controller là cách tiếp cận hỗ trợ nhiều kiểu biểu diễn dữ liệu
![Model-View-Controller](https://db.tt/mOXvkjRO)

Có 2 loại thông tin cần được biểu diễn:

- **Thông tin tĩnh**: Tạo ở lúc bắt đầu và không thay đổi trong phiên làm việc.
- **Thông tin động**: Thay đổi trong phiên làm việc và phải thông báo cho người sử dụng

Các kĩ thuật hiển thị lượng lớn thông tin:
- **Hình ảnh**: có thể cho thấy quan hệ giữa các thực thể và các xu hướng của dữ liệu
- **Màu sắc**: thường dùng để *highlight* các thông tin đặc biệt

Hướng dẫn về việc sử dụng màu sắc:
- Hạn chế số màu và mức độ sặc sỡ
- Dùng sự thay đổi màu để báo hiệu thay đổi trạng thái hệ thống.
- Dùng kí hiệu màu (color coding) để hỗ trợ công việc người dùng đang cố làm. Highlight những điểm người dùng cần chú ý.
- Dùng kí hiệu màu một cách cẩn trọng và nhất quán
- Cẩn thận về hiệu ứng cặp đôi của màu sắc. Một số tổ hợp màu gây khó đọc, ví dụ như người ta không thể cùng lúc chú ý cả hai màu đỏ và xanh lam

4.5: Quy trình thiết kế giao diện
------------

Thiết kế giao diện là một quy trình lặp đi lặp lại với sự liên lạc chặt chẽ giữa người dùng và người thiết kế. Ba hoạt động chính trong quy trình:

- **User analysis**: Tìm hiểu người dùng sẽ làm gì với hệ thống;
- **System prototyping**: phát triển một loạt các bản mẫu để thử nghiệm
- **Interface evaluation**: thử nghiệm các bản mẫu cùng với người dùng

4.6: Quốc tế hóa và địa phương hóa
-----------

Trong quá trình thiết kế cần phải xem xét đến việc ngôn ngữ theo chuẩn quốc tế và chuẩn địa phương. Tức là giao diện phần mềm có thể thích ứng với sự khác nhau về khu vực, ngôn ngữ và yêu cầu kĩ thuật của thị trường.
Quốc tế hóa là quá trình thiết kế một ứng dụng bao gồm nhiều ngôn ngữ để có thể thích nghi với những khu vực không có sự thay đổi quan trọng về quy trình.
Địa phương hóa là sự thích ứng của quốc tế hóa với một khu vực hoặc ngôn ngữ cụ thể bằng cách thêm vào các thành phần của địa phương và dịch văn bản.
Các yếu tố cần được quan tâm như biểu tượng, số, tiền tệ, thời gian và các đơn vị đo lường.

4.7: Biểu tượng và khái niệm quen thuộc
-------------

Người thiết kế giao diện sử dụng các biểu tượng và khái niệm để tạo được sự quen thuộc giữa các phần mềm với những hệ thống đã được biết đến trên thế giới.
Như vậy người dùng sẽ dễ dàng hơn trong việc tìm hiểu và sử dụng giao diện.

*Ví dụ*: Chức năng *xóa tập tin* có thể gắn vào biểu tượng thùng rác.

Khi thiết kế giao diện, nhà thiết kế không được sử dụng nhiều hơn một ý nghĩa, hay chức năng trong một biểu tượng.
Bằng cách sử dụng những biểu tượng và khái niệm quen thuộc, hỗ trợ biểu diễn tốt hơn các thông tin cần được quốc tế hóa, nhưng cần phải chú ý không nên áp dụng theo cùng một cách với tất cả các địa phương và khu vực khác nhau.

5. Phân tích và đánh giá chất lượng thiết kế phần mềm
==============

Phần này gồm các phân tích và đánh giá chất lượng trong thiết kế phần mềm:

- Cần thực hiện một số đánh giá UI để đánh giá mức độ thích hợp
- Đánh giá đầy đủ và toàn bộ thì quá đắt và không thực tế cho hầu hết các hệ thống
- Một giao diện cần được đánh giá theo một đặc tả về tính sử dụng.

5.1: Các thuộc tính về tính sử dụng
---------------

Thuộc tính | Mô tả
---------- | -----
Khả năng học | Người dùng mới cần bao lâu để có thể hoạt động hiệu quả với hệ thống?
Tốc độ vận hành | Tốc độ phản ứng của hệ thống có đáp ứng tốt công việc của người dùng?
Chịu lỗi | Mức độ dung thứ lỗi của hệ thống đối với lỗi người dùng.
Khả năng khôi phục | Khả năng hệ thống khôi phục từ lỗi của người dùng.
Tương thích | Hệ thống gắn bó chặt chẽ với một kiểu làm việc đến đâu?

5.2: Kĩ thuật đánh giá và phân tích
---------------

- Câu hỏi điều tra để lấy phản hồi của người dùng.
- Quay video về việc sử dụng hệ thống rồi sau đó đánh giá nội dung.
- Cài các đoạn mã thu thập thông tin về các tiện ích được sử dụng và lỗi của người dùng.
- Phần mềm có chức năng thu thập phản hồi trực tuyến của người dùng.

5.3: Biện pháp
--------------

Các biện pháp có thể được sử dụng để phân tích và đánh giá các khía cạnh khác nhau của việc thiết kế phần mềm.
Ví dụ: cấu trúc, chất lượng, kích thước, hiệu năng, ...

Các biện pháp này được chia thành 2 loại:

- **Chức năng dựa trên thiết kế**: Chức năng được xây dựng bằng cách phân tích các giao diện của hệ thống, 
- **Thiết kế hướng đối tượng**: Sử dụng lớp các đối tượng làm trung tâm, từ đó xây dựng ra chức năng và giao diện
