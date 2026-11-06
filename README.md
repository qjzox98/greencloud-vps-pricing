# mua vps greencloud: chọn gói đúng nhu cầu, nắm rõ giới hạn ẩn và điều kiện hoàn tiền trước khi xuống tiền

Mua VPS GreenCloud đáng tiền nếu bạn cần một con VPS KVM giá rẻ từ $6/tháng, chạy NVMe/SSD tốc độ cao, và đặc biệt là muốn đặt máy tại Việt Nam (Hà Nội hoặc TP.HCM) với thanh toán qua thẻ ngân hàng trong nước. Ngược lại, nếu mục tiêu chính của bạn là phục vụ người dùng Trung Quốc đại lục, phần lớn gói thường của GreenCloud sẽ làm bạn thất vọng.

Trong bài này mình sẽ đi qua từng dòng sản phẩm đang bán trên trang chính thức, bảng giá đầy đủ, rồi nói kỹ những điều ít bài viết nào nhắc tới: điều kiện hoàn tiền 7 ngày thực ra khá hẹp, port 10Gbps có cơ chế fair-share, và việc nâng cấp dung lượng bị chặn ở một mức nhất định.

> **Chọn nhanh:** Đa số người mới chỉ cần gói **RyzenKVM-1 ($6/tháng)** hoặc **RyzenKVM-2 ($10/tháng)** — Ryzen 3.5GHz+ với NVMe, đủ chạy website, bot, proxy cá nhân. Muốn tiết kiệm tối đa và chấp nhận không hoàn tiền thì Budget KVM Sale từ $25/năm là mức giá hiếm nơi có. 👉 [Xem bảng giá hiện tại của GreenCloud](https://greencloudvps.com/billing/aff.php?aff=6679)

## GreenCloud là nhà cung cấp như thế nào?

GreenCloudVPS (còn gọi ngắn là GreenCloud) thành lập năm 2013, hiện vận hành bởi 365 Group LLC — một công ty LLC đăng ký tại Delaware, Mỹ, sở hữu toàn bộ phần cứng và thiết bị mạng của mình, đồng thời là thành viên của ARIN, APNIC và RIPE. Hệ thống máy chủ trải rộng hơn 30 địa điểm trên 4 châu lục. Điểm mà người Việt sẽ quan tâm nhất: đây là nhà cung cấp gốc Việt, có phòng máy tại **Hà Nội và TP.HCM** (dùng được cho cả dòng Ryzen KVM, Budget KVM lẫn Mac Mini dedicated, tùy tồn kho từng thời điểm), nhận thanh toán qua thẻ ngân hàng Việt Nam, PayPal, thẻ tín dụng, Alipay, UnionPay và tiền mã hóa.

Về uy tín, GreenCloud từng dẫn đầu khảo sát thường niên của cộng đồng LowEndTalk năm 2021 với hai danh hiệu Top Provider và Most Stable Provider — một cộng đồng nổi tiếng khó tính trong giới VPS giá rẻ. Trang bán hàng của họ công bố thời gian phản hồi ticket trung bình khoảng 9–12 phút. Tuy nhiên uy tín này gắn liền với phân khúc "giá rẻ, tự quản" (unmanaged), nghĩa là bạn tự cài đặt, tự xử lý lỗi phần mềm; nhà cung cấp chỉ đảm bảo phần cứng, mạng và uptime đúng cam kết.

SLA chính thức là 99.99% cho mạng và điện, với mức bồi thường tối đa 30 ngày dịch vụ. Con số này viết trong điều khoản, không phải lời quảng cáo suông.

## Bảng giá VPS GreenCloud đầy đủ

Hai dòng KVM VPS tiêu chuẩn của GreenCloud có giá giống hệt nhau: $6, $10, $20, $40 và $80 mỗi tháng, chênh nhau ở loại CPU và ổ cứng. Cả hai đều dùng port 10Gbps, chỉ hỗ trợ Linux, và đi kèm một slot backup/snapshot miễn phí.

**Dòng Ryzen KVM VPS** (CPU Ryzen 3.5GHz+, ổ NVMe):

| Gói | Cấu hình (CPU + ổ) | RAM | Băng thông (APAC / Mỹ-EU) | Giá | Đặt mua |
| --- | --- | --- | --- | --- | --- |
| RyzenKVM-1 | 1 nhân Ryzen @3.5+GHz, 15GB NVMe | 1GB | 750GB / 1.5TB | $6/tháng | [ Mua RyzenKVM-1](https://greencloudvps.com/billing/aff.php?aff=6679) |
| RyzenKVM-2 | 1 nhân Ryzen @3.5+GHz, 30GB NVMe | 2GB | 1TB / 2TB | $10/tháng | [ Mua RyzenKVM-2](https://greencloudvps.com/billing/aff.php?aff=6679) |
| RyzenKVM-3 | 2 nhân Ryzen @3.5+GHz, 50GB NVMe | 4GB | 2TB / 4TB | $20/tháng | [ Mua RyzenKVM-3](https://greencloudvps.com/billing/aff.php?aff=6679) |
| RyzenKVM-4 | 4 nhân Ryzen @3.5+GHz, 80GB NVMe | 8GB | 4TB / 8TB | $40/tháng | [ Mua RyzenKVM-4](https://greencloudvps.com/billing/aff.php?aff=6679) |
| RyzenKVM-5 | 8 nhân Ryzen @3.5+GHz, 150GB NVMe | 16GB | 6TB / 12TB | $80/tháng | [ Mua RyzenKVM-5](https://greencloudvps.com/billing/aff.php?aff=6679) |

**Dòng Budget KVM VPS** (CPU EPYC/E5v4, ổ SSD RAID-10):

| Gói | Cấu hình (CPU + ổ) | RAM | Băng thông (APAC / Mỹ-EU) | Giá | Đặt mua |
| --- | --- | --- | --- | --- | --- |
| SSDKVM-1 | 1 nhân, 15GB SSD RAID-10 | 1GB | 750GB / 1.5TB | $6/tháng | [ Mua SSDKVM-1](https://greencloudvps.com/billing/aff.php?aff=6679) |
| SSDKVM-2 | 1 nhân, 15GB SSD RAID-10 | 2GB | 1TB / 2TB | $10/tháng | [ Mua SSDKVM-2](https://greencloudvps.com/billing/aff.php?aff=6679) |
| SSDKVM-3 | 2 nhân, 30GB SSD RAID-10 | 4GB | 2TB / 4TB | $20/tháng | [ Mua SSDKVM-3](https://greencloudvps.com/billing/aff.php?aff=6679) |
| SSDKVM-4 | 4 nhân, 60GB SSD RAID-10 | 8GB | 4TB / 8TB | $40/tháng | [ Mua SSDKVM-4](https://greencloudvps.com/billing/aff.php?aff=6679) |
| SSDKVM-5 | 8 nhân, 120GB SSD RAID-10 | 16GB | 6TB / 12TB | $80/tháng | [ Mua SSDKVM-5](https://greencloudvps.com/billing/aff.php?aff=6679) |

**Các dòng sản phẩm khác** đang bán trên trang chính (giá khởi điểm, tính theo tháng):

- **EPYC VDS** — máy chủ ảo với nhân CPU vật lý riêng (không chia sẻ): EPYCVDS-1 là 1 nhân EPYC Milan, 8GB RAM, 80GB NVMe, 4TB traffic, giá $10/tháng, có 7 ngày hoàn tiền.
- **Windows VPS** — hai hướng để chọn. Budget Windows bắt đầu từ $8/tháng (1 nhân, 1GB RAM, 25GB SSD, port 1Gbps, traffic không giới hạn, Windows Server 2022); dòng SuperSaving rẻ RAM hơn hẳn cùng mức giá (Budget-1 $10/tháng đã có 2GB RAM) nhưng bắt buộc trả tối thiểu theo quý. Nếu cần băng thông lớn thì dòng 10Gbps Windows khởi điểm $35/tháng (2 nhân, 4GB RAM, 60GB SSD). Trang Budget Windows còn ghi rõ cho phép chạy các công cụ trao đổi traffic kiểu Hitleap/Jingling — điều hầu hết nhà cung cấp cấm.
- **macOS VPS** — MAC-1 $22 (2 nhân/2GB, chỉ Mojave/Catalina), MAC-2 $40, MAC-3 $75, MAC-4 $150, traffic không giới hạn. Làm iOS development cần Xcode mới thì phải bắt đầu từ MAC-2.
- **Mac Mini M4 dedicated** — đặt tại Hà Nội, từ Basic M4 ($160) đến Enterprise M4 Pro ($550), giao trong 1–3 ngày làm việc. VPS thường thì mở trong 15 phút, riêng dòng dedicated server phải chờ.
- **Storage KVM VPS** — ổ HDD lớn dành cho backup và lưu trữ file, có thể mua thêm tối đa 20TB với giá $5/TB/tháng.
- **CN Premium Optimized** — tối ưu cho Trung Quốc đại lục (CN2 GIA), gói Mini $25/tháng, gói cao nhất $320/tháng, có backup hàng ngày, và theo chính trang phân loại là **không hoàn tiền**.

Một điểm nhiều người bỏ qua: cùng giá, **băng thông khu vực APAC thấp hơn Mỹ/EU một nửa**. RyzenKVM-1 ở Singapore/HK/VN chỉ có 750GB, đặt ở Mỹ hoặc châu Âu là 1.5TB. Nếu dịch vụ của bạn phục vụ người dùng toàn cầu, đặt máy tại Mỹ thường "lời" hơn về băng thông.

## Ryzen KVM và Budget KVM khác nhau ở đâu?

Khác nhau ở CPU và ổ cứng; băng thông và giá thì giống nhau. Ryzen KVM dùng CPU Ryzen 3.5GHz+ với ổ NVMe — phù hợp các tác vụ cần tốc độ I/O cao như database, WordPress, ứng dụng web. Budget KVM dùng EPYC (Rome/Milan) hoặc E5v4 đời cũ hơn với SSD RAID-10 — đủ dùng cho nhu cầu thông thường, và theo ghi nhận trên cộng đồng, gói Budget sale 4 nhân/8GB khoảng $45/năm chạy Mastodon, Nextcloud, Redis cùng lúc vẫn ổn.

Nói thẳng: trừ khi bạn cần hiệu năng I/O đỉnh, chênh lệch giữa hai dòng khó cảm nhận được trong đa số trường hợp. Budget KVM Sale dưới đây mới là lý do thật sự để đọc tiếp.

## Budget KVM Sale: rẻ hơn nhiều lần nhưng đổi lại điều gì?

Đây là dòng đặc biệt của GreenCloud với mức giá thấp bất thường: khoảng **$25 cho 12 tháng** (tương đương $2.08/tháng) với cấu hình 4GB RAM, 35GB NVMe RAID-10, 2 nhân EPYC, port 10Gbps. Cùng mức RAM/traffic ở dòng thường là $20/tháng. Lưu ý băng thông tùy vị trí: node Mỹ cho 4TB (bản -2) trong khi node Singapore DC1 chỉ 750GB — đặt gần nhà thì traffic bị cắt mạnh.

Cái giá phải trả nằm ở ba chữ "No refund" in trên chính trang đặt hàng. Gói này không hoàn tiền trong bất kỳ trường hợp nào. Nó cũng tồn tại theo kiểu "mở kho định kỳ" — GreenCloud thả một lượng stock nhất định rồi để hết, chứ không bán quanh năm. Thời điểm khảo sát gần nhất, hầu hết vị trí đã hết hàng, chỉ còn một số node ở Illinois, Florida, Missouri và vài nơi khác còn slot. 👉 [Kiểm tra gói Budget KVM Sale còn hàng ở vị trí nào](https://greencloudvps.com/billing/aff.php?aff=6679)

Điều kiện kèm theo cũng khác gói thường: gói Flash Sale đổi vị trí máy chủ tốn $10/lần, phải active ít nhất 1 tháng, và **gói mua bằng mã giảm giá thì không được đổi vị trí**. APAC chỉ cho đổi trong cùng quốc gia (ví dụ Singapore DC1 ↔ DC2), khác với Mỹ/EU đổi thoải mái trong khu vực.

## Chính sách hoàn tiền 7 ngày: đọc kỹ trước khi mua

"7 ngày hoàn tiền" của GreenCloud có thật, nhưng điều kiện hẹp hơn nhiều người tưởng. Theo điều khoản dịch vụ chính thức, hoàn tiền chỉ áp dụng cho:

1. **Khách hàng mới**, với **gói VPS đầu tiên** của tài khoản
2. Trong vòng **7 ngày** kể từ ngày đăng ký tài khoản
3. Gói **thông thường** (không áp dụng cho gói khuyến mãi, flash sale)

Các trường hợp không được hoàn tiền mà bạn nên nhớ:

- Trả bằng **tiền mã hóa (Bitcoin và các loại crypto)** — mất hoàn toàn quyền hoàn tiền
- Gói khuyến mãi và flash sale
- Đã dùng **từ 10% băng thông trở lên**
- Gói đã bị suspend/terminate vì vi phạm chính sách
- Dedicated server và proxy
- Add-on như cPanel, DirectAdmin

Ngoài ra còn một khoản phí ẩn trong hợp đồng: hóa đơn chậm hơn **2 ngày** sẽ bị tính **10% phí phạt**, dịch vụ có thể bị suspend ngay sau 1 ngày quá hạn và terminate sau 3 ngày. Nếu mua gói Sale giá rẻ để dùng lâu dài, hãy đảm bảo phương thức thanh toán tự động hoạt động tốt — mất máy vì quên thanh toán $2.08/tháng thì hơi oan.

> Muốn "thử rồi quyết định", hãy mua gói Ryzen/Budget KVM thường bằng PayPal hoặc thẻ trong 7 ngày đầu. 👉 [Mở gói RyzenKVM-1 $6/tháng để dùng thử có hoàn tiền](https://greencloudvps.com/billing/aff.php?aff=6679) Đã chọn Budget KVM Sale hoặc trả bằng crypto thì coi như chốt đơn luôn, đừng mua rồi mới tính.

## Những giới hạn ẩn mà trang bán hàng không nói rõ

Đây là phần mà đa số bài đánh giá về GreenCloud bỏ qua, nhưng lại quyết định việc bạn dùng có thoải mái hay không.

**Đường nối tới Trung Quốc đại lục rất yếu (trừ gói CN Premium).** Trang sản phẩm Ryzen của chính GreenCloud ghi chú: VPS Hong Kong nối thẳng về đại lục chỉ có **10Mbps**, Nhật là 1Gbps. Nghĩa là nếu bạn mua VPS Hong Kong giá $10 để "tối ưu cho người Trung Quốc", thì đó là một quyết định sai lầm tốn tiền — đúng hướng thì phải mua CN Premium riêng, bắt đầu từ $25/tháng và không hoàn tiền. Với Tokyo, bạn phải chọn đường truyền SoftBank hoặc IIJ ngay lúc đặt hàng; muốn đổi sau này tốn $10 và IP sẽ thay đổi.

**Port 10Gbps là fair-share, không phải băng thông riêng.** Điều khoản cấm: chạy quá 100Mbps liên tục hơn 6 tiếng, hoặc bung full port thường xuyên. Cũng cấm luôn game server (Counter-Strike, Battlefield), TOR và streaming. Chạy torrent hợp pháp thì chỉ cho phép trên Windows VPS, Storage KVM và dedicated server. Ai định mua VPS để seed hoặc stream thì dừng ở đây.

**Mua thêm băng thông ở APAC đắt gấp 5 lần Mỹ/EU.** Theo điều khoản dịch vụ, port 1Gbps ở Mỹ và châu Âu tính $3/TB/tháng, còn APAC là **$15/TB/tháng**; với port 10Gbps mức phí được liệt kê khác ($4/TB/tháng), nên hãy coi các con số này là tham chiếu và kiểm tra tại thời điểm mua. Nếu ứng dụng của bạn tiêu tốn nhiều traffic, chênh lệch này có thể vượt cả tiền thuê máy.

**Nâng cấp RAM/CPU/ổ có trần.** Giá add-on tiêu chuẩn là $3/1GB RAM, $3/nhân CPU, $3/10GB SSD mỗi tháng, nhưng tối đa chỉ được gấp đôi cấu hình gốc. VPS 4GB RAM nhiều nhất lên 8GB, muốn hơn phải mua gói mới. Riêng gói flash sale có bảng giá add-on riêng rẻ hơn (RAM $1.50/GB, SSD $1/10GB), nhưng tính theo toàn bộ chu kỳ thanh toán.

**Phí đổi IP và đổi vị trí.** Đổi IP tính $2/lần ở Mỹ/EU và $3/lần tại khu vực APAC theo bảng phí trong điều khoản. Đổi vị trí máy chủ $3/lần với gói thường, $10/lần với gói khuyến mãi; APAC chỉ cho đổi trong cùng quốc gia. GreenCloud ghi rõ không bảo đảm truy cập các dịch vụ như Netflix hay Etsy từ IP datacenter; khách Trung Quốc bị GFW chặn IP được đổi miễn phí một lần trong 3 giờ đầu sau khi giao máy.

## Hiệu năng thực tế: số liệu benchmark từ người dùng

GreenCloud mạnh nhất về ổ đĩa, yếu nhất về đường truyền đi châu Âu. Số liệu dưới đây đến từ các bài đánh giá có công bố kết quả đo cụ thể, không phải lời khen chung chung.

Một VPS RyzenKVM Hong Kong (2 nhân Ryzen 9 5950X, 4GB, đo năm 2022) đạt **522 MB/s đọc ghi 4K ngẫu nhiên** với khoảng 130k IOPS, Geekbench 5 đạt 1404 điểm single-core và 2510 multi-core. Cùng kỳ đo, một VPS Hetzner EPYC 2 nhân chỉ đạt khoảng 142 MB/s ở phép thử 4K — chậm hơn gần 4 lần. Với các ứng dụng nặng I/O như database hay nhiều file nhỏ, NVMe của GreenCloud thắng rõ.

Băng thông thì ngược lại. Con máy Hong Kong nói trên chỉ đẩy được khoảng 94 Mbps đến London, 76–93 Mbps đến các điểm ở Mỹ, 187 Mbps đến Tallahassee. Hetzner cùng thời điểm đo tới London 3.73 Gbps. Đến bài đo gần đây hơn ở Singapore DC2 (tháng 8/2026, EPYC Milan), tốc độ nội địa Singapore đạt khoảng 9.2 Gbps — ổn áp trong khu vực — nhưng đi ra châu Âu/Mỹ chỉ quanh 700–900 Mbps.

Kết luận từ số liệu: GreenCloud hợp với dịch vụ phục vụ người dùng châu Á, đặc biệt Việt Nam và Singapore. Website nhắm đến khán giả châu Âu cần băng thông dày thì các nhà cung cấp đặt tại châu Âu sẽ hợp lý hơn về mặt mạng.

## Nên và không nên mua GreenCloud trong trường hợp nào?

**Nên mua khi:**

- Cần VPS giá rẻ cho website cá nhân, blog, bot, VPN riêng, dự án side project — Budget KVM Sale hoặc RyzenKVM-1/2 là đủ
- Muốn đặt máy tại Việt Nam (Hà Nội, TP.HCM) hoặc Singapore với giá thấp hơn hẳn so với các nhà cung cấp lớn
- Cần macOS VPS, Mac Mini M4 dedicated để build iOS, hoặc Windows VPS giá rẻ cho automation — đây là các dòng sản phẩm hiếm, và vị trí Hà Nội giúp latency về Việt Nam thấp
- Muốn thanh toán bằng thẻ ngân hàng trong nước, Alipay hoặc crypto

**Không nên mua khi:**

- Mục tiêu chính là phục vụ người dùng Trung Quốc đại lục mà không sẵn sàng trả $25+/tháng cho CN Premium
- Cần chạy game server, streaming, hoặc băng thông liên tục cao
- Cần hỗ trợ kỹ thuật chi tiết (unmanaged) hoặc cần managed hosting
- Muốn dùng thử bằng crypto payment rồi hoàn tiền — không được

Để so sánh cho công bằng: Hetzner rẻ tương đương ở châu Âu, mạng đến EU/Mỹ mạnh hơn nhiều, nhưng ổ cứng chậm hơn rõ rệt và không có node Việt Nam. Các đánh giá chuyên trang cũng xếp GreenCloud rẻ hơn Vultr hay BandwagonHost ở cùng cấu hình, đổi lại độ ổn định và danh tiếng của hai bên kia được đánh giá cao hơn; DigitalOcean có dashboard thân thiện và kho ứng dụng phong phú hơn. Mỗi bên một hướng; GreenCloud mạnh ở chỗ giá thấp kết hợp vị trí châu Á.

## Câu hỏi thường gặp khi mua VPS GreenCloud

**GreenCloud có hỗ trợ tiếng Việt không?**
GreenCloud là nhà cung cấp gốc Việt và được người dùng Việt đánh giá cao về sự thuận tiện khi thanh toán — nhận thẻ ngân hàng Việt Nam, bên cạnh PayPal, thẻ quốc tế, Alipay, UnionPay và crypto (nhớ là crypto thì mất quyền hoàn tiền). Ticket hỗ trợ chủ yếu xử lý bằng tiếng Anh; một số đánh giá ghi nhận phản hồi trong vòng 24 giờ, trong khi trang bán hàng tự công bố trung bình 9–12 phút — thực tế của bạn có thể nằm giữa hai mức này.

**Mua VPS xong bao lâu thì dùng được?**
VPS thường mở trong 15 phút, tối đa 2 giờ. Mac Mini dedicated mất 1–3 ngày làm việc để giao. Thanh toán qua thẻ hoặc PayPal lần đầu cần xác minh một lần, có thể làm chậm开通 — điền đúng thông tin hóa đơn để tránh bị hệ thống chống gian lận giữ lại.

**Có mã giảm giá nào đang hoạt động không?**
GreenCloud chủ yếu chạy flash sale định kỳ (dịp lễ, Black Friday, kỷ niệm thành lập) thay vì mã giảm giá cố định. Budget KVM Sale bán theo kiểu "kho về là hết". Các mã 30% OFF lưu hành trên các trang tổng hợp mã cần tự kiểm tra trước khi dùng — và nhớ rằng gói mua bằng mã giảm giá sẽ không được đổi vị trí máy chủ.

**Có thể nâng cấp VPS sau này không?**
Được, bằng cách mua add-on: $3/1GB RAM, $3/nhân CPU, $3/10GB SSD mỗi tháng, tối đa gấp đôi cấu hình gốc. Windows VPS thì đắt hơn ($5 cho mỗi đơn vị tương ứng). Dòng Storage VPS có thể thêm tối đa 20TB ổ với $5/TB/tháng.

**VPS GreenCloud đổi IP hoặc đổi vị trí máy chủ thế nào?**
Đổi IP $2/lần ở Mỹ/EU, $3/lần ở APAC. Đổi vị trí máy chủ $3/lần với gói thường, $10/lần với gói khuyến mãi, và APAC chỉ cho đổi trong cùng quốc gia. Tokyo đổi giữa SoftBank ↔ IIJ tốn $10 kèm việc IP thay đổi và phải tự backup trước.

## Chọn gói nào theo nhu cầu của bạn?

Chốt bằng vài tình huống cụ thể:

- **Chỉ cần một VPS rẻ để chạy website, bot, thử nghiệm** → RyzenKVM-1 $6/tháng hoặc SSDKVM-1 $6/tháng, đặt Mỹ/EU để lấy băng thông gấp đôi. Mua trong 7 ngày đầu còn quyền hoàn tiền nếu không ưng.
- **Dịch vụ phục vụ người dùng Việt Nam, cần latency thấp** → đặt Hà Nội hoặc TP.HCM. Đây là lợi thế gần như độc quyền của GreenCloud ở phân khúc giá này.
- **Cần tối đa hiệu quả chi phí, chấp nhận không hoàn tiền** → Budget KVM Sale ~$25/năm, 4GB RAM/2 nhân EPYC, nhớ kiểm tra còn stock ở vị trí bạn muốn và băng thông APAC bị giảm đáng kể.
- **Build iOS app** → MAC-2 $40/tháng trở lên; MAC-1 $22 không cài được Xcode mới. Muốn máy riêng cả bộ thì Mac Mini M4 Basic $160/tháng tại Hà Nội.
- **Chạy automation trên Windows hoặc traffic exchange** → Budget Windows từ $8/tháng; cần RAM nhiều hơn cùng giá thì nhìn sang SuperSaving (tối thiểu trả theo quý).
- **Khách hàng ở Trung Quốc** → bỏ qua gói thường, tính ngay vào CN Premium từ $25/tháng; Hong Kong thường chỉ cho bạn 10Mbps về đại lục.

Trước khi bấm đặt hàng, kiểm tra đúng hai thứ: vị trí máy chủ còn stock không, và phương thức thanh toán có nằm ngoài danh sách không hoàn tiền hay không. 👉 [Đặt VPS GreenCloud theo gói bạn đã chọn](https://greencloudvps.com/billing/aff.php?aff=6679)
