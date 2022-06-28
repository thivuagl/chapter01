# Cơ chế hoạt động của *internet*
Internet là hệ thống thông tin toàn cầu. Internet giúp kết nối hàng tỷ máy tính, thiết bị điện tử thông minh khác nhau. Nên mọi người trên toàn cầu có thể giao tiếp với nhau dễ dàng.
Internet là một mạng lưới cáp vật lý toàn cầu. Có thể bao gồm dây đồng điện thoại, cáp TV, cáp quang.

Khi   truy cập vào 1 trang web, máy tính sẽ gửi yêu cầu qua đường dây này tới máy chủ. Trong đó máy chủ chính là nơi lưu trữ các trang web và hoạt động như ổ cứng của máy tính sử dụng hàng ngày. Khi có lệnh yêu cầu thì máy chủ sẽ truy xuất trang web và đưa ra dữ liệu chính xác trở lại máy tính.

Thao tác truy – xuất dữ liệu này được diễn ra vô cùng nhanh chóng chỉ trong một vài giây.
# Giải thích về protocol của *HTTP/HTTPS*
* ***Http (HyperText Transfer Protocol)*** là giao thức truyền tải siêu văn bản được sử dụng trong www dùng để truyền tải dữ liệu giữa Web server đến các trình duyệt Web và ngược lại. 
Hay có thể hiểu khi   gõ vào 1 địa chỉ vào trình duyệt Web, lúc này trình duyệt Web sẽ gửi 1 yêu cầu qua giao thức Http đến Web server. Web server và sẽ nhận yêu cầu này và trả lại kết quả cho trình duyệt Web.

* ***Https (HyperText Transfer Protocol Secure)*** là giao thức Http có sử dụng thêm SSL (Secure Sockets Layer) để mã hóa dữ liệu trong lúc truyền tải dữ liệu nhầm gia tăng thêm tính an toàn cho việc truyền dữ liệu giữa Web server và trình duyệt Web.
* ***Sự khác biệt giữa giao thức HTTP và HTTPS***
Hiện nay giao thức Https chủ yếu được dùng cho các trang web có giao dịch trực tuyến sử dụng thẻ thanh toán đơn hàng. Nhằm đảm bảo an toàn cho giao dịch, tránh bị lấy mất thông tin trong quá trình thanh toán.
Ngoài ra web sử dụng giao thức Https là 1 tín hiệu để Google xếp hạng từ khóa. Việc này khiến rất nhiều trang Web chuyển qua dùng giao thức Https để Seo được tốt hơn.
Tuy nhiên việc dùng Https sẽ khiến việc truy cập của Website chậm hơn so với Http. Và nhiều trang không có giao dịch trực tuyến hay truyền tải thông tin dữ liệu quan trọng thì thông tin có bị lộ hay không cũng không quá quan trọng.
Nhưng hiện nay Chrome sắp có cảnh báo với những website còn sử dụng Http, và ưu tiên các trang web sử dụng Https.
Để có thể sử dụng giao thức Https thì Website phải có chứng chỉ SSL( Secure sockets layer certificate). Còn không thì sẽ gặp tình trạng hiển thị là kết nối không bảo mật trên trình duyệt Chrome.


# Cơ chế hoạt động của các *browser* và sự *khác nhau* giữa các browser
cấu trúc, thành phần chung và cơ bản nhất của một trình duyệt web, gồm các thành phần (tầng) sau: 
![browser architecture](///browser.png)
Nhiệm vụ của các lớp này như sau:

***User Interface:*** Là tầng cao nhất, nơi tương tác chủ yếu giữa người dùng và trình duyệt, nó bao gồm các thành phần quen thuộc như thanh Address, các nút Reload – Back – Home, Biểu tượng Bookmarks… Những thành phần này không ảnh hưởng đến việc hiển thị của trang mà chủ yếu giúp cho việc tương tác thuận tiện hơn. 

***Browser Engine:*** Đây là tầng nằm giữa và là cầu nối giữa User Interface & Rendering Engine. Tầng này sẽ cung cấp actions để giao tiếp và xử lý dữ liệu từ tầng Rendering Engine lên tầng User Interface và ngược lại, chuyển đổi những hành động người dùng thao tác trên tầng Interface xuống Rendering Engine.

***Rendering Engine (Layout engine):*** Đây là một tầng quan trọng, nó đóng vai trò xử lý (rendering) các thẻ – câu lệnh HTML, CSS, XML, JS để hình thành giao diện (layout) hiển thị lên tầng User Interface, những gì chúng ta sẽ nhìn thấy và tương tác.

***Networking – JavaScript Interpreter – Display UI Backend:***

* Networking: Có nhiệm vụ gọi các giao thức về mạng. Ví dụ như các giao thức HTTP (Hypertext Transfer Protocol).
* UI Backend: Có chức năng xử lý và hiển thị các UI components phổ biến như combo-boxes, textbox, drop-down hiển thị trên web.
* JavaScript interpreter: xử lý và thực thi các đoạn mã JavaScript để hiển thị lên trang web. Đây cũng là một thành phần rất quan trọng ảnh hưởng đến việc hiển thị trang web, do các trang web hiện nay thường cần xử lý và sử dụng khá nhiều mã JavaScript.

***Data persistence:*** Có chức năng lưu trữ thông tin và dữ liệu trên máy local. Những dữ liệu này có thể là Cache, Cookies, localStorage, IndexedDB, WebSQL and FileSystem tùy vào từng hệ thống web.

Các trình duyệt họ dùng những bộ xử lý Rendering Engine không giống nhau nên dẫn đến trang web hiển thị không giống nhau giữa các trình duyệt, cụ thể:
| browser | IE | Firefox | Safari & Chrome | Opera |
| :------- | :-------: | :--------: | :-------------------: | --------: |
| browser engines | Trident Engine | Gecko Engine | WebKit (Note: Chrome uses Blink after version 27) | Presto |

# Cơ chế hoạt động của *DNS và domain*
DNS (Domain Name System – hệ thống phân giải tên miền) là một hệ thống giúp con người và máy tính giao tiếp dễ dàng hơn. Con người sử dụng tên, còn máy tính sử dụng số, DNS chính là một hệ thống giúp biên dịch tên hostname (tên miền) thành số để máy tính có thể hiểu được. Nó giống như ứng dụng Danh Bạ trên điện thoại của   vậy thôi!

Cơ bản, DNS là một hệ thống cơ sở dữ liệu giúp biên dịch tên website thành địa chỉ IP. Thông tin của từng tên miền ứng với địa chỉ IP nào được ghi lại trong một “thư viện danh bạ”, và thư viện này được lưu trên các server tên miền.

DNS hoạt động theo từng bước theo cấu trúc của DNS. Bước đầu tiên gọi là DNS query, một truy vấn để lấy thông tin.
ví dụ tìm kiếm website bằng cách gõ tên miền vào trong web browser (ví dụ, www.google.com). Đầu tiên, DNS server sẽ tìm thông tin phân giải trong filehosts – một file text trong hệ điều hành chịu trách nhiệm chuyển hostname thành địa chỉ IP. Nếu không thấy thông tin, nó sẽ tìm trọng cache – bộ nhớ tạm của phần cứng hay phần mềm. Nơi phổ biến nhất lưu thông tin cache này là  bộ nhớ tạm của trình duyệt và bộ nhớ tạm của Internet Service Providers (ISP). Nếu không nhận được thông tin,   sẽ thấy mã lỗi hiện lên.

Tổng cộng có khoảng 4 loại server tham gia vào trong hệ thống phân giải tên miền
* DNS Recursor
* Root Nameserver
* TLD Nameserver
* Authoritative Nameserver

Domain chính là tên miền. Mỗi một trang web bất kỳ thì đều bao gồm 2 yếu tố chính sau: tên miền và máy chủ lưu trữ web. Trong đó tên miền của   trỏ đến máy chủ lưu trữ trang web.

Mỗi một tên miền khác nhau sẽ được liên kết với một địa chỉ IP tương ứng, vì vậy khi người dùng gõ tên miền vào trình duyệt thông qua mạng máy chủ toàn cầu, máy chủ sẽ dễ dàng tìm kiếm tạo nên Hệ thống tên miền (DNS).

Máy chủ DNS có nhiệm vụ tìm kiếm địa chỉ IP đã được liên kết với tên miền và khi thu thập được thông tin của địa chỉ IP nó sẽ trả về trình duyệt web. Đồng thời yêu cầu dữ liệu về trang web từ máy chủ lưu trữ của miền.

Máy chủ web có nhiệm vụ lưu trữ tất cả các dữ liệu của trang web bao gồm các thư mục, cơ sở dữ liệu và mã HTML của nó. Ngay khi máy chủ lưu trữ gửi dữ liệu trở lại thì trình duyệt web sẽ chuyển đổi nó thành một trang web giúp người dùng dễ dàng truy cập.
# Giải thích về *hosting server*
Hosting là thuật ngữ gọi chung cho Host và Web Hosting. Đây là một không gian tối ưu với dung lượng lớn và đường truyền riêng biệt cho một website, có thể truyền tải và chia sẻ dữ liệu trên không gian đó. Hosting có nhiều loại, nhưng hotsting riêng biệt sẽ mang đến hiệu quả sử dụng cao nhất.

Một hosting chất lượng phải đảm bảo được các tiêu chí về tốc độ, băng thông đường truyền, khả năng chịu tải và dung lượng lưu trữ.
* ***Tốc độ hosting:*** là tốc độ của trang tải. Hosting tốt sẽ giúp người truy cập sử dụng website với thời gian tải lý tưởng chỉ từ 3 đến 5 giây. Để đảm bảo tối ưu hóa Page, hướng tới người tiêu dùng tốt thì tốc độ tải của web được các trang web đầu tư vào marketing online chú ý rất nhiều. Đây cũng là điều kiện tiên quyết để một khách hàng có thiện cảm và truy cập lâu hơn trên website của  .
 Để đảm bảo Hosting có đường truyền tốt, tốc độ cao thì máy chủ phải có cấu hình lớn. Server phải đảm bảo không bị tắc ngẽn. Hiện nay tại Việt Nam,  các website thường chọn Server máy chủ ở Nhật hoặc Singapore
 
* ***Dung lượng hosting:*** Đây chính là dung lượng lưu trữ tùy thuộc vào dung lượng trong ổ cứng máy chủ. Dung lượng   cần sử dụng càng cao thì phải chọn hosting càng lớn. Dung lượng hosting lớn bao nhiêu thì giá thành sẽ tăng bấy nhiêu. Chúng phụ thuộc vào nội dung của website, nếu website của   là website đăng tin bất động sản thì sẽ cần rất nhiều dung lượng để lưu trữ cả hình ảnh và video, hoặc nếu là website giới thiệu công ty thì sẽ không cần phải lưu trữ quá nhiều content. Thường thì dung lượng hosting (Disk space) sẽ dao động từ 1GB đến 10GB. Đây cũng chính là lý do vì sao đội ngũ tối ưu hóa onpage phải chú trọng nhiều đến việc tối ưu hóa ảnh và giảm dung lượng các dữ liệu khi đưa lên web. Điều này sẽ giúp web truy cập nhanh và hạn chế tối đa lưu dượng trên hosting.
* ***Băng thông hosting:***
Dữ liệu trao đổi giữa trang web với người dùng internet gọi là băng thông. 1 file tài liệu mà khách hàng dùng website của   tải về sẽ tương đương với 1MB. Tương đương với 100 khách hàng tải file tài liệu   sẽ mất đi 100MB. Việc cân đối người truy cập và lượng doanh số của website phải được đảm bảo. Nếu không   sẽ chi trả nhiều cho băng thông hosting sẽ làm chênh lệch tiền để duy trì hosting của mình.
* ***Khả năng chịu tải*** của Hosting website thường được tính vào các thời điểm cao điểm. Nếu lượng khách hàng cùng truy cập vào 1 web thì chúng chịu được só lượng người truy cập là bao nhiêu. Vượt quá số lượng này thì website sẽ không thể truy cập được. Một hosting tốt phải đảm bảo được điều này. Đặc biệt là các nhà điều hành website phải tính toán được max truy cập của web mình là bao nhiêu.

***Cách thức hoạt động của Hosting***

Bất cứ một Web hosting services cũng sẽ hoạt động theo các cách thức cơ bản như sau:

* Về phía nhà cung cấp hosting: Cung cấp server lưu trữ cho người sử dụng hostin bằng cách không gian lưu trữ với dung lượng hosting   mua theo gói. Quá trình này sẽ được thực hiện bằng cách chia Server thành những không gian lưu trữ nhỏ. Mỗi gói đăng ký hosting sẽ tương đương với một Server khác nhau. Khi người sử dụng muốn tăng hoặc giảm dung lượng lưu trừ thì nhà cung cấp sẽ điều chỉnh là dung lượng hợp lý cho  .

* Về phía người dùng hosting: Chỉ cần upload các files lên hosting và sử dụng. Việc cấu hình hosting có thể thông qua kết nối internet, gửi địa chỉ IP của hosting hoặc gửi đến tên miền Domain đều được. Khi truy cập thì hosting sẽ trả về những tập tin tương ứng cho người dùng website.