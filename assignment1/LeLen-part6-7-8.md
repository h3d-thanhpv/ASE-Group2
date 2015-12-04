6. Quy ước thiết kế phần mềm
=======

###Tại sao cần có quy ước, ký hiệu chung hay tạo các mô hình trong thiết kế phần mềm?
* Truyền tải được nhiều thông tin về phần mềm đến cho người đọc hơn là dùng những dữ liệu thô như văn bản mô tả phần mềm.
* Mô hình giúp chúng ta tổ chức, trình bày trực quan, thấu hiểu và tạo nên các hệ thống phức tạp
* Tất cả mọi người cùng hiểu được phần mềm được xây dựng và hoạt động như thế nào.

Các loại ký hiệu được sử dụng trong thiết kế phần mềm:
1. Ký hiệu dùng trong thiết kế kiến trúc, tổ chức của phần mềm (static view)
2. Ký hiệu dùng cho quá trình thiết kế chi tiết, hành vi của phần mềm (dynamic view)

6.1. Static view
-----------
Những ký hiệu này được dùng trong phân rã mức cao của thiết kế phần mềm, tức là mô tả cấu trúc, các thành phần chính của phần mềm và sự kết nối giữa chúng.

* Architecture description languages (ADLs) - Ngôn ngữ đặc tả kiến trúc: được sử dụng để mô tả một kiến trúc phần mềm. Có nhiều ngôn ngữ ADL khác nhau được phát triển bởi các tổ chức như Wrigh (được phát triển bởi Carnegie Mellon), ACME (Carnegie Mellon), xADL (UCI), Darwin (Imperial College London), DAOP-ADL (Trường đại học Málaga - Tây Ban Nha). Các thành phần cơ bản của một ngôn ngữ ADL là thành phần, kết nối và cấu hình hệ thống.
* Class and object diagrams - Biểu đồ lớp: mô tả quan sát tĩnh của hệ thống thông qua các lớp và các mối quan hệ của chúng
* Component diagrams - Biểu đồ thành phần: biểu đồ mô tả các thành phần và sự phụ
thuộc của chúng trong hệ thống. Các thành phần của hệ thống có thể là mã nguồn, thành phần mã nhị phân (tệp mã đích, thư viện,...) và thành phần thực thi.
* Class responsibility collaborator cards (CRCs): được dùng trong thiết kế hướng đối tượng, sử dụng để biểu thị tên của các thành phần (class) cùng với trách nhiệm và các thành phần hợp tác với nó. CRCs ban đầu được đề xuất bởi Ward Cunningham và Kent Beck như một công cụ giảng dạy, sau được phát triển và sử dụng trong thực tế thiết kế phần mềm.
* Deployment diagrams - Biểu đồ triển khai chỉ ra cấu hình các phần tử xử lý lúc chương trình chạy, các nút trên mạng và các tiến trình phần mềm thực hiện trên những phần tử đó. Nó chỉ ra mối quan hệ giữa các phần cứng và phần mềm của hệ thống. Biểu đồ triển khai chỉ ra toàn bộ các nút trên mạng, kết nối giữa chúng và các tiến trình chạy trên
chúng.
* Entity-relationship diagrams (ERDs) - Sơ đồ thực thể quan hệ: được sử dụng để đại diện cho mô hình khái niệm dữ liệu lưu trữ trong kho thông tin.
* Interface description languages (IDLs) - Ngôn ngữ mô tả giao diện: ngôn ngữ lập trình được sử dụng để xác định các giao diện (tên và các loại xuất khẩu hoạt động) của các thành phần phần mềm.
* Structure charts - Biểu đồ cấu trúc: Chúng được sử dụng trong lập trình có cấu trúc để sắp xếp module của chương trình vào một cái cây. Mỗi mô-đun được đại diện bởi một cái hộp, trong đó có tên của module. Cấu trúc cây biểu thị mối quan hệ giữa các module.
