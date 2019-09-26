# **TÌm Hiểu Về Network**
## **Mục Lục**
- **1.Network là gì,phân loại netword,các thành phần cơ bản của network**
- **2.Tìm hiểu về Network Diagram**
- **3.Network public và private,ip**
- **4.Mô hình *Peer to Peer* và *Client-server***
- **5.Tìm hiểu về *Router*,*Hub*,*Switch***

### **1.Network là gì,phân loại netword,các thành phần cơ bản của network**
- Networks(Mạng): là một mô hình bao gồm nhiều thành phần, các thành phần cơ bản nhất bao gồm các máy tính, thiết bị Router và Switch. Router dùng để truyền thông tin giữa các máy tính không cùng một mạng.
- Phân loại Network ta có thể chia như sau 
 - Theo diện hoạt động 
   - 1.*LAN* (Local Access Network – Mạng truy nhập cục bộ):là một mạng dữ liệu tốc độ cao bao phủ trong một phạm vi địa lý nhỏ  
     - ví dụ như một phòng học, căn nhà, hoặc 1 tòa nhà hoặc một khu phức hợp.
- ![ảnh minh hoạ](https://imgur.com/GRfnN3I.png)
  - 2.*WAN* (Wide Area Network – Mạng diện rộng):là một tập hợp các LAN kết nối với nhau thông qua công nghệ WAN hoặc Internet. Giải pháp sử dụng công nghệ WAN là thuê nhà cung cấp dịch vụ (kênh thuê riêng Leased Line, VPN,…) hoặc sử dụng internet.
- ![ảnh minh hoạ](https://imgur.com/vAoRgOg.png)
  - 3.*MAN* (Metropolitan Area network- Mạng đô thị):là "mạng đô thị", là mạng có cỡ lớn hơn LAN, phạm vi vài km. Nó có thể bao gồm nhóm các văn phòng gần nhau trong thành phố, nó có thể là công cộng hay tư nhân
- ![ảnh minh hoạ](https://imgur.com/OLybfFj.png)
  - 4.*GAN* (Global Area network- Mạng toàn cầu): là mạng của các mạng WAN, trải rộng trên phạm vi toàn cầu 
- ![ảnh minh hoạ](https://imgur.com/WsKsbxZ.png)
      - Ví dụ: các công ty hoạt dông trên nhiều nước trên thế giới , mạng toàn cầu **Internet** cũng là một **GAN** đặc biệt
  - 5.*PAN* (Personal Area network-Mạng các nhân): là mạng chỉ sử dụng trong đình đình
 - Theo mô hình ghép nối
   - 1.*Ponit-to-Point*(mô hình điểm-điểm): mạng gồm nhiều nút mỗi nút chỉ có thể liển lạc với nút liền kề qua đường truyền trực tiếp, mạng có thể bao gồm hàng ngàn nút mỗi nút nối trực tiếp với một nút nào đó.
     - Ví dụ: mô hình mạng **Star**(hình sao) và **Tree**(cây)
- ![ảnh minh hoạ](https://imgur.com/tgQGVxn.png)
  - 2.*Broadcast*(mô hình điểm- nhiều điểm): mạng gồm vác nút dùng chung một kê truyền thông. Khác với mô hình điểm-điểm , dữ liệu từ một máy gửi đi sẽ được truyền đến tất cả các nít tham gia kênh truyền dùng chung. Trong mô hình này cũng có các kiểu truyền thông điệp khác nhau như là *unicast*,*multicast*,*broadcast*
    - Ví dụ: mô hình mạng **BUS** và **RING**
- ![ảnh minh hoạ](https://imgur.com/wNedJDo.png)
 - Theo kiểu chuyển 
   - 1.*Circuit-switched*(chuyển mạch ảo):phải thiết lập mạch vật lý giữa nút nguồn và nút địch trước khi chuyền dữ liệu thực sự, mạch này tồn tại trong suốt thời gian chuyển dữ liệu
- ![ảnh minh hoạ](https://imgur.com/ZOxFszj.png)
  - 2.*Packet-switched network*(chuyển mạch gói): thông điệp đầu tiên được chia thành những đơn vị nhỏ hơn gọi là gói (Packet), sau những lần packet lần lượt gửi tới nút nhận qua mạng lưới các thiết bị chuyển mạch trung gian(Switch)
- ![ảnh minh hoạ](https://imgur.com/7yg1z41.png)

- Các thành phần cơ bản của Network
  - Có ít nhất 2 máy tính
  - Một giao tiếp mạng trên mỗi máy tính(NIC: Network interface Card)
  - Môi Trường Truyền
    - Có dây(dây cáp mạng)
    - Không dây
  - Hệ điều hành( Windows,Unix v.v)
- [link tham khảo thêm 1:](http://tuvancongnghe.net/kien-thuc-mang-may-tinh-co-ban-phan-1-tong-quan-ve-mang-may-tinh/)
- [link tham khảo thêm 2:](https://vi.wikipedia.org/wiki/M%E1%BA%A1ng_m%C3%A1y_t%C3%ADnh) 
### **2.Tìm hiểu về Network Diagram**
- Network Diagram là sơ đồ mạng công việc . Nó là một đồ thị biểu diễn thứ tự/sự phụ thuộc các gói công việc của đề án dưới dạng mạng.
- ![ảnh minh hoạ](https://imgur.com/en4ReJd.png)
- Ràng buộc: mõi công việc phải có một công việc trước và sau trừ hai công việc đầu và cuối
- Các loại quan hệ 
  -  FS :  A kết thúc B bắt đầu .
  -  SS :  A bắt đầu B bắt đầu .
  -  SF :  A bắt đầu B kết thúc .
  -  FF :  A kết thúc B kết thúc .
- Các loại sử dụng mạng công việc
 - Action On Node : công việc trên nút được dùng nhiều trong các ứng dụng thuộc hệ thống thông tin, các ngành công nghiệp thiết kế và mua bán .
 - Action On Arrow : công việc trên cạnh được dùng trong các ứng dụng xây dựng, kĩ thuật này sử dụng các hoạt động giả không tốn tài nguyên .
### **3.Network public và Network private,ip**
- Network Public:Public Network hiểu đơn giản có nghĩa là mạng công cộng. Theo như mặc định của chế độ mạng *Public Network*, tức là khi bạn chưa can thiệp hay chỉnh sửa gì thì khi kết nối internet, máy tính của bạn sẽ không hiển thị các tập tin đã được chia sẻ trong máy tính và người khác sẽ không nhìn thấy những gì bạn chia sẻ trên mạng Lan.Chế độ Puclic Network sẽ ngăn chặn việc chia sẻ tập tin, máy in… và thậm chí là tính năng *HomeGroup* cũng sẽ không hoạt động ở chế độ này. 
 - Ví dụ: như quán càfê , các điểm phát wifi miễn phí, quán game, sân bay …
- Network private(bao gồm *Home Network* và *Work Network*): là mạng tư nhân, thích hợp khi sử dụng trong gia đình, công ty… Theo mặc định, nếu như bạn lựa chọn Private Network thì Windows nó sẽ hiểu ” à đây là đây là một mạng an toàn và đáng tin cậy “. Chính vì vậy mà các thiết bị hay máy tính khác có thể dễ dàng nhìn thấy máy tính của bạn trong mạng Lan và bạn có thể chia sẻ file qua mạng Lan cho người khác rất dễ dàng. 
- ![ảnh minh hoạ](https://imgur.com/dPsbwie.png)
- ![ảnh minh hoạ](https://imgur.com/gIF4DtX.png)
- [link tham khảo](https://blogchiasekienthuc.com/thu-thuat-may-tinh/su-khac-nhau-giua-public-network-va-private-network.html)
- IP: là một địa chỉ đơn nhất mà những thiết bị điện tử hiện nay đang sử dụng để nhận diện và liên lạc với nhau trên mạng máy tính bằng cách sử dụng giao thức Internet.Đến thời điểm hiện tại có loại địa chỉ IP là IPV4(32bit) và IPV6(128bit)
- ![ảnh minh hoạ](https://imgur.com/V3PdczO.png)
- [link tham khảo về ip](https://vi.wikipedia.org/wiki/%C4%90%E1%BB%8Ba_ch%E1%BB%89_IP)
### **4.Kiến trúc mạng ,mô hình *Peer to Peer* và *Client-server***
- **Kiến Trúc Mạng**:Cách nối các máy tính với nhau ra sao và tập hợp các qui tắc, qui ước mà tất cả các thực thể tham gia truyền thông trên mạng phải tuân theo. 
  - Gồm 2 thành phần:
    - Cách nối: Đồ hình mạng (Network Topolopy)
    - Qui tắc, qui ước: Giao thức mạng (Network Protocol)
- **Mô hình *Peer to Peer***:là mạng đồng đẳng, là một mạng máy tính trong đó hoạt động của mạng chủ yếu dựa vào khả năng tính toán và băng thông của các máy tham gia chứ không tập trung vào một số nhỏ các máy chủ trung tâm như các mạng thông thường. Mạng đồng đẳng thường được sử dụng để kết nối các máy thông qua một lượng kết nối dạng ad hoc.Một mạng đồng đẳng đúng nghĩa không có khái niệm máy chủ và máy khách, nói cách khác, tất cả các máy tham gia đều bình đẳng và được gọi là peer, là một nút mạng đóng vai trò đồng thời là máy khách và máy chủ đối với các máy khác trong mạng.
- ![ảnh minh hoạ](https://imgur.com/nRHy6Qd.png)
- [link tham khảo về mạng peer to peer](https://vi.wikipedia.org/wiki/M%E1%BA%A1ng_ngang_h%C3%A0ng)
- **Client-server**:là một mô hình nổi tiếng trong mạng máy tính, được áp dụng rất rộng rãi và là mô hình của mọi trang web hiện có. Ý tưởng của mô hình này là máy con (đóng vài trò là máy khách) gửi một yêu cầu (request) để máy chủ (đóng vai trò người cung ứng dịch vụ), máy chủ sẽ xử lý và trả kết quả về cho máy khách
- ![ảnh minh hoạ](https://imgur.com/4XiDfhF.png)
- [link tham khảo về mạng Client-server](https://vi.wikipedia.org/wiki/Client-server)
- So sánh giữa mạng Peer to Peer và Client-server
- ![ảnh minh hoạ](https://imgur.com/5RUsSMh.png)
### **5.Tìm hiểu về *Router*,*Hub*,*Switch***
- **Router** :là một thiết bị hoạt động trên tầng mạng, nó có thể tìm được đường đi tốt nhất cho các gói tin qua nhiều kết nối để đi từ trạm gửi thuộc mạng đầu đến trạm nhận thuộc mạng cuối. Router có thể được sử dụng trong việc nối nhiều mạng với nhau và cho phép các gói tin có thể đi theo nhiều đường khác nhau để tới đích. Để có thể tìm được các đường đi tốt nhất cho các gói tin mỗi router sẽ có một bàng định tuyến riêng của mình và được update liên tục nhờ vào một số giao thức đinh tuyến cho router như là *RIP*,*OSPF*,*EiGRP*
- ![ảnh minh hoạ](https://imgur.com/mb6t92l.png)
- **Hub**:thường được dùng để nối mạng, thông qua những đầu cắm của nó người ta liên kết với các máy tính dưới dạng hình sao.
 - Người ta chia HUB làm 3 loại như sau:
  - **Hub bị động (Passive Hub)** : Hub bị động không chứa các linh kiện điện tử và cũng không xử lý các tín hiệu dữ liệu, nó có chức năng duy nhất là tổ hợp các tín hiệu từ một số đoạn cáp mạng. Khoảng cách giữa một máy tính và Hub không thể lớn hơn một nửa khoảng cách tối đa cho phép giữa 2 máy tính trên mạng . Các mạng ARCnet thường dùng Hub bị động
    - Ví Dụ: khoảng cách tối đa cho phép giữa 2 máy tính của mạng là 200m thì khoảng cách tối đa giữa một máy tính và hub là 100m
  - **Hub chủ động (Active Hub)** : Hub chủ động có các linh kiện điện tử có thể khuyếch đại và xử lý các tín hiệu điện tử truyền giữa các thiết bị của mạng. Qúa trình xử lý tín hiệu được gọi là tái sinh tín hiệu, nó làm cho tín hiệu trở nên tốt hơn, ít nhạy cảm với lỗi do vậy khoảng cách giữa các thiết bị có thể tăng lên. Tuy nhiên những ưu điểm đó cũng kéo theo giá thành của Hub chủ động cao hơn nhiều so với Hub bị động. Các mạng Token ring có xu hướng dùng Hub chủ động
  - **Hub thông minh (Intelligent Hub)**: cũng là Hub chủ động nhưng có thêm các chức năng mới so với loại trước, nó có thể có bộ vi xử lý của mình và bộ nhớ mà qua đó nó không chỉ cho phép điều khiển hoạt động thông qua các chương trình quản trị mạng mà nó có thể hoạt động như bộ tìm đường hay một cầu nối. Nó có thể cho phép tìm đường cho gói tin rất nhanh trên các cổng của nó, thay vì phát lại gói tin trên mọi cổng thì nó có thể chuyển mạch để phát trên một cổng có thể nối tới trạm đích.
- **Switch**:hay còn gọi là thiết bị chuyển mạch, là một thiết bị dùng để kết nối các đoạn mạng với nhau theo mô hình mạng hình sao (star). Theo mô hình này, switch đóng vai trò là thiết bị trung tâm, tất cả các máy tính đều được nối về đây.Switch làm việc như một Bridge nhiều cổng. Khác với Hub nhận tín hiệu từ một cổng rồi chuyển tiếp tới tất cả các cổng còn lại, switch nhận tín hiệu vật lý, chuyển đổi thành dữ liệu, từ một cổng, kiểm tra địa chỉ đích rồi gửi tới một cổng tương ứng.Trong mô hình tham chiếu OSI, switch hoạt động ở tầng liên kết dữ liệu, ngoài ra có một số loại switch cao cấp hoạt động ở tầng mạng.
- ![ảnh minh hoạ](https://imgur.com/5ad0PBl.png)


