                                            BÁO CÁO BÀI TẬP LỚN MÔN LẬP TRÌNH MẠNG 
                                                HỌC KỲ I  NĂM HỌC 2022  - 2023
                                                          Nhóm: 03_07
1. Giới thiệu sơ lược chủ đề

a. Mục tiêu
    - Tạo 1 app Video Streaming cho phép chia sẻ video:
    - Client có thể gửi lên server các video, sau đó Server lưu trữ video tại đó thành một cái kho lưu trữ Video
    - Client Khi client yêu cầu xem 1 video nào đó, server gửi về video cho client xem và có thao tác cho từng video:
    - Client gửi yêu cầu Play thì Server gửi về mở trình phát video, còn khi ấn Pause thì tạm dừng video
    - Ngôn ngữ sử dụng: Java

b. kết quả đã đạt được
    - Tạo được 1 phần client gửi 1 video lên server quan giao thức RTSP
    - Tạo được trình phát cho 1 video

c. Hạn chế, hướng phát triển
    - Hạn chế: Chưa tạo được cách client gửi lên server theo nhiều đuôi video khác nhau
    - Hướng phát triển: Tạo 1 kho lưu trữ video trên server, client có thể vào xem video

2. Tổng hợp công việc

----------------------------------------------------------------------------------------------------------------------------------------------
  STT   |        MSV - Họ tên           |  Các nội dung thực hiện      |          Thể hiện           |      Ghi chú
----------------------------------------------------------------------------------------------------------------------------------------------
   1    | B19DCCN623 - Lê Tài Tuệ       |  12/10/2022 đến 19/10/2022   |     VideoStream.java        | tạo lớp VideoStream.java, 
        |                               |                              |                             |  Chuyển đổi dữ liệu Byte thành các mảng
----------------------------------------------------------------------------------------------------------------------------------------------
   2    | B19DCCN040 - Phan Quốc Anh    |  12/10/2022 đến 19/10/2022   | ClientVideoStreaming.java,  | Tạo được 1 cái Client gửi video
        |                               |                              | ServerVideoStreaming.java   | lên Server  và trình phát cho 1 video
        |                               |                              |                             | bằng giao thức RTP và RTSP
----------------------------------------------------------------------------------------------------------------------------------------------    
   3    | B19DCCN188 - Đỗ Minh Đức      |  12/10/2022 đến 19/10/2022   | RTPPacket.java              | Tạo lớp cho giao thức RTP
----------------------------------------------------------------------------------------------------------------------------------------------




3. Quá trình phát triển

----------------------------------------------------------------------------------------------------------------------------------------------
  STT   |   Phiên bản  |      Vấn đề          |       Xử lý                 |     thư viện/Công cụ |  Tự đánh giá |       Người thực hiện
----------------------------------------------------------------------------------------------------------------------------------------------
   1    | 1.0 15/10    |  Client gửi file     |    Tạo 1 hàm có đủ các yêu  |      Java.io.Socket  |     Ok       |   Đỗ Minh Đức, Lê Tài Tuệ
                       |  Video lên Server    |    cầu của giao thức        |                      |              |   Phan Quốc Anh
                       |                      |    RTSP để gửi              |                      |              |
----------------------------------------------------------------------------------------------------------------------------------------------
   2    | 2.0 19/10    | Trình phát cho video |   Tạo các hàm và xử lý cho  |      Java.io.Socket  |     Ok       |   Đỗ Minh Đức, Lê Tài Tuệ
                       |  Video lên Server    |   cầu của giao thức         |                      |              |    Phan Quốc Anh
                       |                      |  từng chức năng Play, Pause |                      |              |
----------------------------------------------------------------------------------------------------------------------------------------------



4. Mã nguồn:  https://github.com/PQAnhPtit/Video-Streaming.git