<h1>Thiết kế phần mềm</h1>
<h2>Giới thiệu</h2>
<p>
Khái niệm thiết kế được định nghĩa theo 2 cách sau:</br>
<li>
  <b>Thiết kế</b> là quy trình định nghĩa ra kiến trúc, thành phần, interfaces và các thuộc tính khác của một hệ thống hoặc một thành phần. 
  Trong quy trình này, yêu cầu phần mềm được phân tích để đưa ra một cấu trúc của phần mềm làm cơ sở để làm ra phần mềm. 
</li>
<li>
  <b>Thiết kế</b> là kết quả của một quá trình. Nó mô tả kiến trúc của một phần mềm như là phần mềm được phân rã và tổ chức như thế nào trong các thành phần và các interfaces giữa các thành phần như thế nào. Nó cũng có thể mô tả các thành phần ở mức chi tiết cho phép có thể xây dựng được phần mềm
</li>
</p>
<p>
<b>Thiết kế phần mềm</b> đóng vai trò quan trọng: trong quá trình thiết kế, những kỹ sư phần mềm sẽ đề xuất các mô hình cụ thể là các bản vẽ thiết kế là giải pháp giải quyết vấn đề và thực hiện được. Chúng ta có thể phân tính và đánh giá những mô hình này có hay không phù hợp với những yêu cầu khác nhau
Đầu ra của thiết kế phần mềm sẽ được sử dụng cho quá trình xây dựng và kiểm thử nên việc đánh giá một thiết kế có phù hợp hay không rất quan trọng, nếu một thiết kế sai sẽ dẫn đến tất cả các quá trình sau đó cũng sai và cần phải chỉnh sửa nếu thiết kế được chỉnh sửa.
</p>
<p>
Thiết kế phần mềm gồm 2 hoạt động:
<li><b>Thiết kế kiến trúc</b> (còn được gọi là thiết kế mức cao): là phát triển mức kiến trúc cao nhất và đưa ra cách tổ chức phần mềm và chỉ ra các thành phần khác nhau trong phần mềm</li>
<li><b>Thiết kế chi tiết</b>: chỉ ra chi tiết và đầy đủ về thành phần tạo điều kiện xây dựng phần mềm trong pha sau đó</li>
<h2>1. Nguyên tắc thiết kế phần mềm cơ bản</h2>
<p>
Phần này đưa ra khái niệm, quan niệm và thuật ngữ hình thành nền tảng cơ bản để hiểu biết về vai trò và phạm vi của thiết kế phần mềm
</p>
<h3>1.1	Khái niệm thiết kế chung </h3>
<p>Trong nhận thức thông thường, thiết kế có thể được xem như là một hình thức giải quyết vấn đề.</p>
<h3>1.2	Bối cảnh của thiết kế phần mềm</h3>
<p>Thiết kế phần mềm là một phần quan trọng của quy trình phát triển phần mềm. Thiết kế phần mềm sẽ quyết định mô hình phát triển cũng như các hoạt động xây dựng phần mềm, kiểm thử phần mềm và bảo trì phần mềm.</p>
<h3>1.3	Quy trình thiết kế phần mềm</h3>
<p>
Thiết kế phần thường được xem như là một quy trình 2 bước:
<li>Thiết kế kiến trúc (cũng được xem như là thiết kế mức cao high-level design or top-level design) mô tả phầm mềm được tổ chức thành các thành phần như thế nào</li>
<li>Thiết kế chi tiết mô tả hành động mong muốn của những thành phần</li>
</p>
<p>Đầu ra của 2 quy trình này là tập mô hình và tài liệu ghi lại những những quyết định quan trọng đã được thực hiện cùng lời giải thích cho mỗi lý do. Bằng cách ghi lại các lý do đó công việc bảo trì dài hạn của phần mềm được nâng cao</p>
<h3>1.4	Nguyên tắc thiết kế phần mềm</h3>
<p>Nguyên tắc là “một giả định, giáo lý hoặc luật cơ bản và toàn diện”. Nguyên tắc thiết kế phần mềm là quan niệm chính cung cấp kiến thức cơ bản cho khái niệm và hướng tiếp cận thiết kế phần mềm khác nhau. Nguyên tắc thiết kế phần mềm bao gồm trừu tượng hóa; ghép nối và liên kết; phân rã và modul hóa; đóng gói/ẩn thông tin; tách giao diện và thực hiện; đầy đủ, toàn vẹn và nguyên thủy; và tách mối quan tâm (separation of cencerns)</p>
<li><b>Abstraction</b>: là một cách nhìn của một đối tượng mà tập trung vào thông tin liên quan để cụ thể hóa mục đích và tránh bỏ xót thông tin”. Trong bối cảnh của thiết kế phần mềm, 2 cơ chế trừu tượng hóa chìa khóa là tham số hóa và cụ thể hóa. Trừu tượng bởi tham số hóa trừu tượng từ biểu diễn dữ liệu chi tiết bởi biểu diễn dữ liệu như tên những tham số. Trừu tượng hóa bởi cụ thể hóa dẫn đến 3 loại trừu tượng: trừu tượng thủ tục, trừu tượng dữ liệu và trừu tượng điều khiển (trừu tượng tương tác lẫn nhau)</li>
<li><b>Coupling and Conhesion</b>: Ghép nối là một độ đo của độ phụ thuộc lẫn nhau giữa các module trong chương trình máy tính, trong khi đó liên kết là độ đo độ mạnh của mối liên kết giữa các phần tử trong một module.</li>
<li><b>Phân rã hóa và module hóa</b>: Phân rã hóa và modul hóa nghĩa là phần mềm lớn được chia thành một số thành phần định danh (dễ định nghĩa interface) mà mô tả tương tác giữa các thành phần. Thông thường mục tiêu là thay thế những chức năng và trách nhiệm trong những thành phần khác nhau.</li>
<li><b>Đóng gói và ẩn thông tin</b>: nghĩa là nhóm và đóng gói chi tiết bên trong của một trừu tượng và làm cho những chi tiết không thể được truy cập từ bên ngoài</li>
<li><b>Tách giao diện và thực hiện</b> liên quan đến việc xác định mọt thành phần bằng cách xác định một giao diện public (được biết đến như là client) mà là tách từ chi tiết của thành phần được hiện thực hóa như thế nào.</li>
<li><b>Tính đầy đủ, toàn vẹn và nguyên thủy</b>: mục tiêu của tính đầy đủ, toàn vẹn và nguyên thủy nghĩa là chắc rằng một thành phần chỉ tương ứng với những đặc điểm quan trọng của một trừu tượng. Nguyên thủy nghĩa là thiết kế nên được dựa trên mô hình dễ thực hiện</li>
<li>Tách liên quan. Một liên quan là một “khu vực quan tâm với sự liên quan đến thiết kế phần mềm”. Một liên quan thiết kế là một lĩnh vực của thiết kế mà liên quan đến một hay nhiều các bên liên quan. Mỗi kiến trúc nhìn một hay nhiều khung nhìn liên quan. Tác liên quan bởi những khung nhìn cho phép quan tâm các bên liên quan để tập trung vào một việc tại một thời điểm và yêu cầu và cung cấp một phương tiện quản lý phức tạp</li>
<h2>2.	Những vấn đề chính trong thiết kế kiến trúc phần mềm</h2>
Một số vấn đề quan trọng phải được xử lý trong khi thiết kế phần mềm. Đặc biệt là những lo ngại về chất lượng phần mềm mà có thể kể đến như: hiệu suất, bảo mật, độ tin cậy, khả năng sử dụng, vv. Một số vấn đề quan trọng khác là làm thế nào để phân rã, tổ chức và đóng gói những thành phần phần mềm. Đây là nguyên tắc cơ bản mà tất các các phương pháp thiết phải giải quyết nó bằng cách này hay cách khác. Ngược lại, những vấn đề “liên quan đến các khía cạnh của các hành vi phần mềm mà lại không nằm trong miền ứng dụng mà nằm ở các miền khác có liên quan” Những vấn đề đó thường xuyên chồng chéo với các chức năng của hệ thống và được gọi những khía cạnh mà đa phần không phải là đơn vị phân rã của phần mềm mà là thuộc tính ảnh hưởng đến hiệu suất hoặc ngữ nghĩa của các thành phần một cách có hệ thống.
<h3>2.1	Tương tranh (concurrency)</h3>
<p>Thiết kế cho tương tranh là có liên quan đến phân rã phần mềm thành quy trình, nhiệm vụ, quá trình và đối phó với các vấn đề liên quan đến tính hiệu quả, tính nguyên tố, đồng bộ hóa và lập kế hoạch</p>
<h3>2.2	Điều khiển và xử lý các sự kiện</h3>
<p>Vấn đề thiết kế này liên quán tới làm thế nào tổ chức dữ liệu và dòng dữ liệu cũng như làm thế nào để xử lý các sự kiện tạm thời và phản xạ qua các cơ chế lời gọi ngầm và gọi lại.</p>
<h3>2.3	Dữ liệu bền vững (data persistence)</h3>
<p>Vấn đề của thiết kế này liên quan tới làm thế nào để xử lý dữ liệu tồn tại lâu dài</p>
<h3>2.4	Phân phối các thành phần</h3>
<p>Vấn đề của thiết kế này liên quan đến làm thế nào để phân phối các phần mềm trên phần cứng ( bao gồm phần cứng máy tính và phần cứng mạng), làm thế nào các thành phần giao tiếp được với nhau, và làm thế nào tầng giữa có thể được sử dụng để đối phó với không tương thích phần mềm.</p>
<p>2.5	Lỗi và xử lý ngoại lệ và lỗi dung nạp (error and exception handling and fault tolerance)</p>
<p>Vấn đề của thiết kế này liên quan đến làm thế nào để phòng chống, chịu đựng và các xử lý lỗi và đối phó với các điều kiện ngoại lệ<p>
<h3>2.6	Tương tác và trình bày (Interaction and presentation)</h3>
<p>Vấn đề thiết kế này liên quan tới làm thế nào để cấu trúc và tổ chức tương tác với những người dùng và biểu diễn thông tin ( ví dụ, chia giao diện và khung nhìn logic sử dụng hướng tiếp cận MVC)</p>
<p>Chú ý rằng chủ đề này không chỉ chi tiết giao diện người dùng, đó là nhiệm vụ của thiết kế giao diện người dùng</p>
<h3>2.7	Bảo mật (sercurity)</h3>
<p>Thiết kế cho bảo mật liên quan đến làm thế nào để ngăn chặn tiết lộ trái phép, sáng tạo, thay đổi, xóa, hoặc từ chối truy cập đến thông tin từ các nguồn khác. Nó cũng quan tâm làm thế nào để chịu được các cuộc tấn công bảo mật hoặc sự xâm phạm bởi hạn chế thiệt hại, tiếp tục dịch vụ, tốc độ sữa chữa và phục hồi, và thất bại và phục hồi an toàn. Kiểm soát truy cập là một khái niệm an ninh cơ bản và ta cũng nên đảm bảo sử dụng đúng mật mã</p>
<h2>3.	Kiến trúc và cấu trúc phần mềm</h2>
<p>Một kiến trúc phần mềm là “tập hợp các cấu trúc cần thiết để suy luận về hệ thống, trong đó bao gồm các yếu tố phần mềm, mối quan hệ giữa chúng và đặc tính của cả hai. Trong suốt những năm 1990, tuy nhiên, kiến trúc phần mềm bắt đầu nổi lên như một ngành học rộng liên quan đến việc nghiên cứu các cấu trúc phần mềm và kiến trúc theo một cách chung chung. Điều đó dẫn đến một số khái niệm thú vị về thiết kế phần mềm tại những mức độ khác nhau của trừu tượng hóa. Mội số khái niệm có thể hữu ích trong việc thiết kế kiến trúc ( ví dụ phong cách kiến trúc) cũng như trong suốt thiết kế chi tiết (ví dụ design pattern). Những khái niệm thiết kế này cũng được sử dụng để thiết kế những chương trình tương tự.</p>
<h3>3.1	Cấu trúc và viewpoints</h3>
<p>Khía cạnh mức cao khác nhau của thiết kế phần mềm có thể được mô tả và tài liệu hóa. Những khía cạnh này thường được gọi là các góc nhìn “Một góc nhìn biểu diễn một phần khía cạch của kiến trúc phần mềm mà biểu diễn cụ thể chính xác của hệ thống phần mềm”. Các góc nhìn thích hợp với những vấn đề khác nhau liên quan đến phần mềm – ví dụ, góc nhìn logic (đáp ứng các yêu cầu chức năng) với góc nhìn tiến trình (vấn đề đồng thời) với góc nhìn vật lý (vấn đề phân phối) với góc nhìn phát triển (làm thế nào để thiết kế được break down thành các thành phần đơn vị với đại diện rõ ràng của sự phụ thuộc giữa các đơn vị). Nhiều tác giả sử dụng những thuật ngữ khác nhau- như góc nhìn hành vi, góc nhìn chức năng, góc nhìn cấu trúc, góc nhìn mô hình dữ liệu. Tóm lại, thiết kế phần mềm là nhiều khía cạnh sản xuất bởi quá trình thiết kế và cấu tạo từ quan điểm độc lập tương đối và những góc nhìn trực giao.</p>
<h3>3.2	Kiểu kiến trúc</h3>
<p>Kiểu kiến trúc là một chuyên môn hóa của phần tử và các loại liên quan, cùng với một bộ những hạn chế về cách nó có thể được sử dụng. Môt vài tác giải chỉ ra một số kiểu kiến trúc chính như sau:
<li>Kiến trúc thường (ví dụ, phân tâng, pipes and filter, blackboard)</li>
<li>Các hệ thống phân tán (ví dụ client-server, three-tiers, broker)</li>
<li>Các hệ thống tương tác (ví dụ, MVC, Presentation-Abstraction-Control, WPF)</li>
<li>Các hệ thống mô phỏng (ví dụ, microkernel, reflection)</li>
<li>Các kiểu khác (ví dụ, batch, interperters, process control, rule-based)</li>
</p>
<h3>3.3	Mẫu thiết kế (Design Patterns)</h3>
<p>Mẫu là một giải pháp phổ biến để giải quyết các vấn đề phồ biến trong ngữ cảnh đưa ra. Trong khi kiểu kiến trúc có thể được nhìn như mẫu mô tả tổ chức mức cao của phần mềm, mẫu thiết kế có thể sử dụng mô tả cụ thể ở mức thấp. Những mẫu thiết kế mức thấp bao gồm:
<li>Mẫu tạo (ví dụ, builder, factory, prototype, singleton)</li>
<li>Mẫu cấu trúc (ví dụ, adapter, bridge, composite, decorator, façade, fly-weight, proxy)</li>
<li>Mẫu hành vi (ví dụ, command, interperter, iterator, mediator, memento, observer, state, strategy, template, visitor)</li>
</p>
<h3>3.4	Những quyết định thiết kế kiến trúc</h3>
<p>Thiết kế kiến trúc là một quá trình sáng tạo. Trong suốt quy trình thiết kế, nhà thiết kế phần mềm phải tạo một số quệt định cơ bản ảnh hưởng sâu sắc tới các phát mềm và quy trình phát triển phần mềm. Nó rất hữu ích để suy nghĩa quy trình thiết kế phần mềm từ quan điểm làm quyết định hơn là từ quan điểm hoạt động. Thông thường, tác động vào chất lượng thuộc tính và hoán đổi giữa các thuốc tính cạnh trạnh là cơ sở cho quyết định thiết kế</p>
<h3>3.5	Tương tự giữa chương trình và framework</h3>
<p>Một cách tiếp cận cung cấp cho việc sử dụng lại thiết kế phần mềm và thành phần là sử dụng những chương trình tương tự. Điều này có thể thực hiện bằng xác định sự tương đồng giữa các phần mềm bằng cách thiết kế các thành phần tái sử dụng và tùy vào sự khác nhau giữa các phần mềm. Trong lập trình hướng đối tượng, một khái niệm chìa khóa có liên quan đến khung là một khung: một phần hệ thống phần mềm hoàn toàn có thể được mở rộng bằng cách cài đặt các công cụ thích hợp</p>

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

6. Quy ước thiết kế phần mềm
-----------

###Tại sao cần có quy ước, ký hiệu chung hay tạo các mô hình trong thiết kế phần mềm?
* Truyền tải được nhiều thông tin về phần mềm đến cho người đọc hơn là dùng những dữ liệu thô như văn bản mô tả phần mềm.
* Mô hình giúp chúng ta tổ chức, trình bày trực quan, thấu hiểu và tạo nên các hệ thống phức tạp
* Tất cả mọi người cùng hiểu được phần mềm được xây dựng và hoạt động như thế nào.

Các loại ký hiệu được sử dụng trong thiết kế phần mềm:

1.  Ký hiệu dùng trong thiết kế kiến trúc, tổ chức của phần mềm (**static view**).
2.  Ký hiệu dùng cho quá trình thiết kế chi tiết, hành vi của phần mềm (**dynamic view**).

###6.1. Static view

Những ký hiệu, mô hình này được dùng trong phân rã mức cao của thiết kế phần mềm, tức là mô tả cấu trúc, các thành phần chính của phần mềm và sự kết nối giữa chúng. Dưới đây là một số mô hình thường dùng trong thiết kế phần mềm ở mức cao.

  * **Architecture description languages (ADLs) - Ngôn ngữ đặc tả kiến trúc**: được sử dụng để mô tả một kiến trúc phần mềm. Có nhiều ngôn ngữ ADL khác nhau được phát triển bởi các tổ chức như Wrigh (được phát triển bởi Carnegie Mellon), ACME (Carnegie Mellon), xADL (UCI), Darwin (Imperial College London), DAOP-ADL (Trường đại học Málaga - Tây Ban Nha). Các thành phần cơ bản của một ngôn ngữ ADL là thành phần, kết nối và cấu hình hệ thống.
  * **Class and object diagrams - Biểu đồ lớp**: mô tả quan sát tĩnh của hệ thống thông qua các lớp và các mối quan hệ của chúng
  * **Component diagrams - Biểu đồ thành phần**: biểu đồ mô tả các thành phần và sự phụ
thuộc của chúng trong hệ thống. Các thành phần của hệ thống có thể là mã nguồn, thành phần mã nhị phân (tệp mã đích, thư viện,...) và thành phần thực thi.
  * **Class responsibility collaborator cards (CRCs)**: được dùng trong thiết kế hướng đối tượng, sử dụng để biểu thị tên của các thành phần (class) cùng với trách nhiệm và các thành phần hợp tác với nó. CRCs ban đầu được đề xuất bởi Ward Cunningham và Kent Beck như một công cụ giảng dạy, sau được phát triển và sử dụng trong thực tế thiết kế phần mềm.
  * **Deployment diagrams - Biểu đồ triển khai**: chỉ ra cấu hình các phần tử xử lý lúc chương trình chạy, các nút trên mạng và các tiến trình phần mềm thực hiện trên những phần tử đó. Nó chỉ ra mối quan hệ giữa các phần cứng và phần mềm của hệ thống. Biểu đồ triển khai chỉ ra toàn bộ các nút trên mạng, kết nối giữa chúng và các tiến trình chạy trên
chúng.
  * **Entity-relationship diagrams (ERDs) - Sơ đồ thực thể quan hệ**: được sử dụng để đại diện cho mô hình khái niệm dữ liệu lưu trữ trong kho thông tin.
  * **Interface description languages (IDLs) - Ngôn ngữ mô tả giao diện**: ngôn ngữ lập trình được sử dụng để xác định các giao diện (tên và các loại xuất khẩu hoạt động) của các thành phần phần mềm.
  * **Structure charts - Biểu đồ cấu trúc**: Chúng được sử dụng trong lập trình có cấu trúc để sắp xếp module của chương trình vào một cái cây. Mỗi mô-đun được đại diện bởi một cái hộp, trong đó có tên của module. Cấu trúc cây biểu thị mối quan hệ giữa các module.

###6.2. Dynamic view

Có nhiều loại ký hiệu, mô hình dùng cho qúa trình thiết kế chi tiết đang được áp dụng phổ biến hiện nay.
  * **Activity diagram - Sơ đồ  hoạt động**: Biểu đồ hoạt động tập trung vào công việc được thực hiện trong khi thực thi một thủ tục (hàm). Nó nắm bắt hành động (công việc và những hoạt động phải được thực hiện) cũng như kết quả của chúng theo sự biến đổi trạng thái.
  * **Communication diagram - Biểu đồ giao tiếp**: được sử dụng để hiển thị sự tương tác xảy ra trong một nhóm của các đối tượng; trọng tâm là về đối tượng, các liên kết và những trao đổi giữa chúng.iếp
  * **Data flow diagrams (DFDs) - Sơ đồ luồng dữ liệu**: một công cụ mô tả mối quan hệ thông tin giữa các đối tượng, cung cấp bức tranh tổng thế của hệ thống và một thiết kế sơ bộ về thực hiện các chức năng. Biều đồ luồng dữ liệu có thể được sử dụng để phân tích an ninh, vì nó cung cấp các hướng có thể tấn công và tiết lộ thông tin bí mật.
  * **Decision tables and diagrams - Bảng và biểu đồ quyết định**: sử dụng để mô tả sự kết hợp phức tạp của các hành động trong phần mềm.
  * **Flowcharts - Biểu đồ tiến trình (lưu đồ)**: Frank Gilbreth thành viên của ASME ( the American Society of Mechanical Engineers) giới thiệu lần đầu năm 1921. Nó mô tả một quá trình bằng cách sử dụng những hình ảnh hoặc những ký hiệu kỹ thuật ... nhằm mô tả đầy đủ nhất đầu ra và dòng chảy của quá trình, tạo điều kiện cho việc điều tra các cơ hội cải tiến bằng việc hiểu biết chi tiết về quá trình làm việc của nó.
  * **Sequence diagrams - Biểu đồ tuần tự**: minh họa các đối tượng tương tác với nhau ra sao. Chúng tập trung vào các chuỗi thông điệp được gửi và nhận giữa các đối tượng.
  * **State transition and state chart diagrams - Biểu đồ trạng thái**: nắm bắt vòng đời của các đối tượng, các hệ thống con (Subsystem) và các hệ thống. Chúng cho ta biết các trạng thái mà một đối tượng có thể có và các sự kiện (các thông điệp nhận được, các khoảng thời gian đã qua đi, các lỗi xảy ra, các điều kiện được thỏa mãn) sẽ ảnh hưởng đến những trạng thái đó như thế nào dọc theo tiến trình thời gian
  * **Formal specification languages - Ngôn ngữ đặc tả chính thức**: ngôn ngữ văn bản mà sử dụng các khái niệm cơ bản từ toán học (ví dụ, logic, thiết lập, trình tự) để xác định một cách chặt chẽ và trừu tượng phần mềm giao diện thành phần và hành vi.
  * **Pseudo code and program design languages (PDLs) - Mã giả và ngôn ngữ thiết kế chương trình**: cấu trúc ngữ lập trình như
ngôn được sử dụng để mô tả, thiết kế chi tiết, hành vi của một phần mềm hoặc phương pháp.

7. Chiến lược và phương pháp thiết kế phần mềm
-----------
Có nhiều chiến lược hỗ trợ cho quá trình thiết kế qua các phương pháp tiếp cận khác nhau. Tuy nhiên chẳng có một chiến lược nào tốt nhất cho các dự án. Hai chiến lược thiết kế đang được dùng rộng rãi và cho thấy hiệu quả tích cực là thiết kế hướng chức năng và thiết kế hướng đối tượng. Mỗi chiến lược đều có những ưu, nhược điểm riêng phụ thuộc vào ứng dụng phát triển và nhóm phát triển phần mềm. Hai cách tiếp cận này là bổ sung và hỗ trợ cho nhau chứ không đối kháng nhau.

###7.1 Thiết kế hướng chức năng

Thiết kế hướng chức năng là một cách tiếp cận thiết kế phần mềm trong đó bản thiết kế được phân giải thành một bộ các đơn thể được tác động lẫn nhau, mà mỗi đơn thể có một chức năng được xác định rõ ràng. 

Đây là một phương pháp cổ điển. Người ta dùng các biểu đồ dòng dữ liệu mô tả việc xử lý dữ liệu logic, các lược đồ cấu trúc để chỉ ra cấu trúc của phần mềm và mối quan hệ giữa các thành phần.

Thiết kế hướng chức năng gắn với các chi tiết của một thuật toán của chức năng nhưng các thông tin trạng thái của hệ thống không bị che dấu. Điều này có thể gây ra vấn đề khi một chức năng thay đổi trạng thái theo cách mà các chức năng khác không ngờ tới thì hệ thống sẽ trục trặc. Do đó cách tiếp cận chức năng để thiết kế là thắng lợi nhất khi mà khối lượng thông tin trạng thái của hệ thống là nhỏ nhất và thông tin dùng chung nhau là rõ ràng nhất.

###7.2. Thiết kế hướng đối tượng.

Hệ thống được nhìn nhận như một bộ các đối tượng, phân tán, mỗi đối tượng có những thông tin trạng thái riêng của nó. 

  * Thiết kế hướng đối tượng là dựa trên việc che dấu thông tin do dữ liệu dùng chung bị loại bỏ. Các đối tượng liên lạc với nhau bằng cách trao đổi thông báo. 
  * Các đối tượng là các thực thể độc lập, sẵn sàng thay đổi mà không ảnh hưởng tới các đối tượng khác.
  * Các đối tượng có thể phân tán và hành động tuần tự hoặc song song.

**Ưu điểm**
  - Dễ bảo trì và các đối tượng là độc lập.
  - Có thể dùng lại một số thành phần của đối tượng đã được thiết kế trước đó.
  - Thiết kế dễ hiểu: nhìn rõ được mối quan hệ giữa các thực thể

**Nhược điểm**
  - Cách nhìn tự nhiên nhiều hệ thống là cách nhìn chức năng nên việc thích nghi với cách nhìn đối tượng đôi khi là khó khăn. Làm sao để tìm ra các đối tượng thích hợp trong một hệ thống cũng là một vấn đề khó khăn.

###7.3. Thiết kế lấy cấu trúc dữ liệu làm trung tâm

Các kỹ sư phần mềm cần mô tả các đầu vào và đầu ra cấu trúc dữ liệu và sau đó phát triển cấu trúc điều kiển của chương trình dự trên các sơ đồ cấu trúc dữ liệu. 

###7.4. Thiết kế hướng thành phần

Một thành phần phần mềm là một đơn vị độc lập,có giao diện và phụ thuộc có thể được triển khai một cách độc lập. Chiến lược thiết kế hướng thành phần dựa trên các vấn đề liên quan đến việc cung cấp, phát triển, và tích hợp các thành phần như vậy để cải thiện, tái sử dụng. Tái sử dụng và off-the-shelf thành phần phần mềm phải đáp ứng các yêu cầu bảo mật tương tự như phần mềm mới. Quản lý tin tưởng là một mối quan tâm thiết kế; thành phần được coi có một mức độ nhất định của sự tin cậy không nên phụ thuộc vào các thành phần ít đáng tin cậy hay dịch vụ.

###7.5. Các phương pháp khác
Ngoài các hướng thiết kế trên còn nhiều hướng thiết kế khác cũng đang được áp dụng hiện nay và mang lại những hiệu quả nhất định. Gần đây xuất hiện một kiến trúc phần mềm mới được kỳ vọng là chìa khóa giải quyết vấn đề "đơn giản hóa" phần mềm là SOA (Service-Oriented Architecture) - kiến trúc hướng dịch vụ.  SOA là tập hợp các dịch vụ kết nối “mềm dẻo” với nhau, có giao tiếp được định nghĩa rõ ràng và độc lập với nền tảng hệ thống, và có thể tái sử dụng. SOA là cấp độ cao hơn của phát triển ứng dụng, chú trọng đến quy trình nghiệp vụ và dùng giao tiếp chuẩn để giúp che đi sự phức tạp kỹ thuật bên dưới.
Nói cách khác, SOA là:

  * Một kiểu kiến trúc phần mềm gồm nhiều thành phần độc lập được thể hiện thành những dịch vụ (service), mỗi dịch vụ thực hiện quy trình nghiệp vụ nào đó của doanh nghiệp.
  * Các thành phần được nối kết qua cổng giao tiếp, có tính kế thừa các thành phần đang tồn tại, và sự tương tác giữa chúng không cần quan tâm đến việc chúng được phát triển trên nền tảng công nghệ nào. Điều này khiến hệ thống có thể mở rộng và tích hợp một cách dễ dàng.

SOA giúp tái sử dụng phần mềm, linh hoạt khi mở rộng, kết nối và tích hợp.

8. Công cụ thiết kế phần mềm
-----------
Công cụ thiết kế phần mềm có thể được sử dụng để hỗ trợ tạo ra các mô hình phần mềm trong quá trình phát triển phần mềm. Nó có thể giúp việc thiết kế phần mềm trở lên rõ ràng, linh hoạt và hiệu quả hơn.
  * Chuyển các yêu cầu phần mềm thành một mô hình thiết kế trực quan.
  * Cung cấp mô tả từ tổng quan đến chi tiết từng thành phần của phần mềm và giao diện của nó
  * Trợ giúp cho quá trình đánh giá chất lượng phần mềm.

Một số công cụ thiết kế phần mềm đang được sử dụng nhiều hiện nay ở Việt Nam: StarUML, Rational Rose, ...
