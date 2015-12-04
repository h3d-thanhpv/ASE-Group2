6. Quy ước thiết kế phần mềm
-----------

###Tại sao cần có quy ước, ký hiệu chung hay tạo các mô hình trong thiết kế phần mềm?
* Truyền tải được nhiều thông tin về phần mềm đến cho người đọc hơn là dùng những dữ liệu thô như văn bản mô tả phần mềm.
* Mô hình giúp chúng ta tổ chức, trình bày trực quan, thấu hiểu và tạo nên các hệ thống phức tạp
* Tất cả mọi người cùng hiểu được phần mềm được xây dựng và hoạt động như thế nào.

Các loại ký hiệu được sử dụng trong thiết kế phần mềm:

1.  Ký hiệu dùng trong thiết kế kiến trúc, tổ chức của phần mềm (*static view*).
2.  Ký hiệu dùng cho quá trình thiết kế chi tiết, hành vi của phần mềm (*dynamic view*).

###6.1. Static view

Những ký hiệu, mô hình này được dùng trong phân rã mức cao của thiết kế phần mềm, tức là mô tả cấu trúc, các thành phần chính của phần mềm và sự kết nối giữa chúng. Dưới đây là một số mô hình thường dùng trong thiết kế phần mềm ở mức cao.

  * *Architecture description languages (ADLs) - Ngôn ngữ đặc tả kiến trúc*: được sử dụng để mô tả một kiến trúc phần mềm. Có nhiều ngôn ngữ ADL khác nhau được phát triển bởi các tổ chức như Wrigh (được phát triển bởi Carnegie Mellon), ACME (Carnegie Mellon), xADL (UCI), Darwin (Imperial College London), DAOP-ADL (Trường đại học Málaga - Tây Ban Nha). Các thành phần cơ bản của một ngôn ngữ ADL là thành phần, kết nối và cấu hình hệ thống.
  * *Class and object diagrams - Biểu đồ lớp*: mô tả quan sát tĩnh của hệ thống thông qua các lớp và các mối quan hệ của chúng
  * *Component diagrams - Biểu đồ thành phần*: biểu đồ mô tả các thành phần và sự phụ
thuộc của chúng trong hệ thống. Các thành phần của hệ thống có thể là mã nguồn, thành phần mã nhị phân (tệp mã đích, thư viện,...) và thành phần thực thi.
  * *Class responsibility collaborator cards (CRCs)*: được dùng trong thiết kế hướng đối tượng, sử dụng để biểu thị tên của các thành phần (class) cùng với trách nhiệm và các thành phần hợp tác với nó. CRCs ban đầu được đề xuất bởi Ward Cunningham và Kent Beck như một công cụ giảng dạy, sau được phát triển và sử dụng trong thực tế thiết kế phần mềm.
  * *Deployment diagrams - Biểu đồ triển khai*: chỉ ra cấu hình các phần tử xử lý lúc chương trình chạy, các nút trên mạng và các tiến trình phần mềm thực hiện trên những phần tử đó. Nó chỉ ra mối quan hệ giữa các phần cứng và phần mềm của hệ thống. Biểu đồ triển khai chỉ ra toàn bộ các nút trên mạng, kết nối giữa chúng và các tiến trình chạy trên
chúng.
  * *Entity-relationship diagrams (ERDs) - Sơ đồ thực thể quan hệ*: được sử dụng để đại diện cho mô hình khái niệm dữ liệu lưu trữ trong kho thông tin.
  * *Interface description languages (IDLs) - Ngôn ngữ mô tả giao diện*: ngôn ngữ lập trình được sử dụng để xác định các giao diện (tên và các loại xuất khẩu hoạt động) của các thành phần phần mềm.
  * *Structure charts - Biểu đồ cấu trúc*: Chúng được sử dụng trong lập trình có cấu trúc để sắp xếp module của chương trình vào một cái cây. Mỗi mô-đun được đại diện bởi một cái hộp, trong đó có tên của module. Cấu trúc cây biểu thị mối quan hệ giữa các module.

###6.2. Dynamic view

Có nhiều loại ký hiệu, mô hình dùng cho qúa trình thiết kế chi tiết đang được áp dụng phổ biến hiện nay.
  * *Activity diagram - Sơ đồ  hoạt động*: Biểu đồ hoạt động tập trung vào công việc được thực hiện trong khi thực thi một thủ tục (hàm). Nó nắm bắt hành động (công việc và những hoạt động phải được thực hiện) cũng như kết quả của chúng theo sự biến đổi trạng thái.
  * *Communication diagram - Biểu đồ giao tiếp*: được sử dụng để hiển thị sự tương tác xảy ra trong một nhóm của các đối tượng; trọng tâm là về đối tượng, các liên kết và những trao đổi giữa chúng.iếp
  * *Data flow diagrams (DFDs) - Sơ đồ luồng dữ liệu*: một công cụ mô tả mối quan hệ thông tin giữa các đối tượng, cung cấp bức tranh tổng thế của hệ thống và một thiết kế sơ bộ về thực hiện các chức năng. Biều đồ luồng dữ liệu có thể được sử dụng để phân tích an ninh, vì nó cung cấp các hướng có thể tấn công và tiết lộ thông tin bí mật.
  * *Decision tables and diagrams - Bảng và biểu đồ quyết định*: sử dụng để mô tả sự kết hợp phức tạp của các hành động trong phần mềm.
  * *Flowcharts - Biểu đồ tiến trình (lưu đồ)*: Frank Gilbreth thành viên của ASME ( the American Society of Mechanical Engineers) giới thiệu lần đầu năm 1921. Nó mô tả một quá trình bằng cách sử dụng những hình ảnh hoặc những ký hiệu kỹ thuật ... nhằm mô tả đầy đủ nhất đầu ra và dòng chảy của quá trình, tạo điều kiện cho việc điều tra các cơ hội cải tiến bằng việc hiểu biết chi tiết về quá trình làm việc của nó.
  * *Sequence diagrams - Biểu đồ tuần tự*: minh họa các đối tượng tương tác với nhau ra sao. Chúng tập trung vào các chuỗi thông điệp được gửi và nhận giữa các đối tượng.
  * *State transition and state chart diagrams - Biểu đồ trạng thái*: nắm bắt vòng đời của các đối tượng, các hệ thống con (Subsystem) và các hệ thống. Chúng cho ta biết các trạng thái mà một đối tượng có thể có và các sự kiện (các thông điệp nhận được, các khoảng thời gian đã qua đi, các lỗi xảy ra, các điều kiện được thỏa mãn) sẽ ảnh hưởng đến những trạng thái đó như thế nào dọc theo tiến trình thời gian
  * *Formal specification languages - Ngôn ngữ đặc tả chính thức*: ngôn ngữ văn bản mà sử dụng các khái niệm cơ bản từ toán học (ví dụ, logic, thiết lập, trình tự) để xác định một cách chặt chẽ và trừu tượng phần mềm giao diện thành phần và hành vi.
  * *Pseudo code and program design languages (PDLs) - Mã giả và ngôn ngữ thiết kế chương trình*: cấu trúc ngữ lập trình như
ngôn được sử dụng để mô tả, thiết kế chi tiết, hành vi của một phần mềm hoặc phương pháp.

7. Chiến lược và phương pháp thiết kế phần mềm
-----------
Có nhiều chiến lược hỗ trợ cho quá trình thiết kế qua các phương pháp tiếp cận khác nhau. Chẳng có một chiến lược nào tốt nhất cho các dự án. Hai chiến lược thiết kế đang được dùng rộng rãi và cho thấy hiệu quả tích cực là thiết kế hướng chức năng và thiết kế hướng đối tượng. Mỗi chiến lược đều có những ưu, nhược điểm riêng phụ thuộc vào ứng dụng phát triển và nhóm phát triển phần mềm. Hai cách tiếp cận này là bổ sung và hỗ trợ cho nhau chứ không đối kháng nhau.

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
