# POW (proof-of-work)
Proof of Work (thường viết tắt là PoW) là một thuật toán đồng thuận được sử dụng để ngăn chặn tấn công 51% hoặc chi tiêu kép. Tiền điện tử như Bitcoin đang sử dụng PoW đồng thuận để xác nhận giao dịch và sản xuất khối mới thêm vào chuỗi. Với PoW, thợ đào cạnh tranh để hoàn thành giao dịch trên mạng lưới để đổi lấy phần thưởng cho tốc độ và độ chính xác của họ.

# Ưu và Nhược Điểm của PoW

## Ưu Điểm

- Tránh được tấn công DDoS.

- Công bằng và minh bạch.

- Giới hạn tác động của các phần crypto nhỏ do thợ đào nắm giữ.

- Thu hút cộng đồng bằng việc duy trì một mạng lưới lành mạnh.

## Nhược Điểm

- Chi phí lớn để sắm các thiết bị máy tính chuyên nghiệp, thiết bị ngoại vi, và tiêu thụ điện năng.

- Các phép toán phức tạp không có giá trị trong giáo dục hay các công việc hàng ngày, chỉ hữu dụng khi kiểm định khối.

- Nó khiến blockchain tập trung hóa hơn là phi tập trung.

- Việc đào sẽ giảm dần khi phần thưởng không còn hấp dẫn nữa.
- Rủi ro 51% : Nếu một thực thể kiểm soát sở hữu 51% hoặc hơn 51% số nút trong mạng, thì thực thể đó có thể làm hỏng chuỗi khối bằng cách giành được phần lớn mạng.

==> Là cơ chế đồng thuận nguyên thủy, PoW giới thiệu một lý thuyết trò chơi về đám đông, phân phối tính toán, đồng thuận xã hội, kinh tế thị trường, và bằng chứng mật mã học. Nó tạo ra công nghệ blockchain, cho phép các mạng lưới hoạt động với tính bảo mật, bền vững, phân phối đồng thuận. 

Dù thế nào thì sẽ ngày càng nhiều blockchain chuyển sang PoS trong tương lai - PoW đánh dấu một phát minh nổi bật trong tính toán và thiết kế lý thuyết trò chơi.


# PoS (proof-of-stake)

- Proof of Stake (POS) là một thuật toán đồng thuận của blockchain. Có thể hiểu, đây là Bằng chứng ký gửi hay Bằng chứng cổ phần. Trong đó, các Node phải Stake coin để tham gia xác nhận các giao dịch trên block. Nói một cách đơn giản, Node phải gửi coin để xác minh danh tính của nó.

## MộT số thuật ngữ liên quan đến Proof of Stake
- Node (Masternode)
 Node được hiểu là những cá nhân hay tổ chức tham gia xác nhận giao dịch hoặc đóng block của một đồng coin. Dựa trên phương pháp chạy các phần mềm chuyên dụng của đồng coin đó, node đóng vai trò giữ ổn định trong blockchain, xác nhận giao dịch cho người dùng coin.

- Validator
Có thể hiểu Validator là người kiểm định. Theo thuật toán POS, không phải tất cả các node đều tham gia đóng block mới. Blockchain sẽ chọn ngẫu nhiên một node để kiểm định và đóng block.

- Forge hoặc Mint
Là cụm từ chỉ hoạt động kiểm định và đóng block của Validator. Nó dùng để phân biệt với mine (đào) trong POW.

- Stake
Để trở thành một Validator trong Proof of Stake, node phải stake (đặt cọc) một lượng coin nhất định làm điều kiện tham gia. Ý nghĩa của việc này nhằm chứng minh bạn có sở hữu coin.

- Lock và Unlock
Số coin đặt cọc của node sẽ được mạng lưới lock. Trong thời gian trở thành validator, số coin stake này không được di chuyển, hay giao dịch được. Nếu không làm validator nữa thì coin mới được unlock.

## Ưu điểm và nhược điểm của Proof of Stake
### Ưu điểm
Tiết kiệm năng lượng: So với Proof of Work việc khai thác các loại tiền tệ kỹ thuật số trên Proof of Stake có thể tiết kiệm năng lượng hơn rất nhiều vì Proof of Stake chỉ cần máy tính có internet và online 24/24 thì bạn đã có thể đào được rồi.
- Dễ dàng sinh lời: Lãi suất rất ổn định, được xem là mỏ vàng cho các Holder.
- Tính bảo mật cao: Khả năng tấn công 51% và tấn công độc hại lên mạng lưới POS khó khăn hơn rất nhiều. Đặc biệt, nếu các nút kiểm duyệt cố tình xác nhận các giao dịch phi pháp, họ sẽ bị trừ đi phần lớn số tài sản đang nắm giữ
Stake an toàn 100% vì trong ví luôn có bản back up.
- Tính linh hoạt: Nếu node được chọn để làm validator cho block tiếp theo không có mặt trong một khoảng thời gian xác định, thì Proof of Stake sẽ chọn ra các node dự trữ khác có sẵn để ngăn việc treo xử lý
### Nhược điểm
- Mức lãi không chính xác tuyệt đối: Khi staking bạn có thể nhận được mức lãi không như ước tính ban đấu
Có thể lỗ: Nếu tỉ giá Stake thấp hơn tỉ lệ trượt giá của coin thì bạn sẽ lỗ.
- Rủi ro bị scam, lừa đảo: điều này có thể xảy ra khi bạn lựa chọn nền tảng staking không uy tín, hoặc lựa chọn coin “rác”
- Phụ thuộc vào “nhà giàu”: Proof of Stake dựa trên cổ phần tương ứng với nắm giữ. Đồng nghĩa những người nắm giữ token lớn có ROI tốt hơn được xem là “người giàu”. Đồng thời, họ cũng có quyền lực lớn đe dọa quá trình xác thực phi tập trung của mạng.

# So sánh Ưu điểm và nhược điểm của Proof of Stake
### Ưu điểm
- Tiết kiệm năng lượng: So với Proof of Work việc khai thác các loại tiền tệ kỹ thuật số trên Proof of Stake có thể tiết kiệm năng lượng hơn rất nhiều vì Proof of Stake chỉ cần máy tính có internet và online 24/24 thì bạn đã có thể đào được rồi.
- Dễ dàng sinh lời: Lãi suất rất ổn định, được xem là mỏ vàng cho các Holder.
- Tính bảo mật cao: Khả năng tấn công 51% và tấn công độc hại lên mạng lưới POS khó khăn hơn rất nhiều. Đặc biệt, nếu các nút kiểm duyệt cố tình xác nhận các giao dịch phi pháp, họ sẽ bị trừ đi phần lớn số tài sản đang nắm giữ
Stake an toàn 100% vì trong ví luôn có bản back up.
- Tính linh hoạt: Nếu node được chọn để làm validator cho block tiếp theo không có mặt trong một khoảng thời gian xác định, thì Proof of Stake sẽ chọn ra các node dự trữ khác có sẵn để ngăn việc treo xử lý
### Nhược điểm
- Mức lãi không chính xác tuyệt đối: Khi staking bạn có thể nhận được mức lãi không như ước tính ban đấu
- Có thể lỗ: Nếu tỉ giá Stake thấp hơn tỉ lệ trượt giá của coin thì bạn sẽ lỗ.
- Rủi ro bị scam, lừa đảo: điều này có thể xảy ra khi bạn lựa chọn nền tảng staking không uy tín, hoặc lựa chọn coin “rác”
- Phụ thuộc vào “nhà giàu”: Proof of Stake dựa trên cổ phần tương ứng với nắm giữ. Đồng nghĩa những người nắm giữ token lớn có ROI tốt hơn được xem là “người giàu”. Đồng thời, họ cũng có quyền lực lớn đe dọa quá trình xác thực phi tập trung của mạng.


# DPos(Delegated Proof of Stake)
 Delegated Proof of Stake (DPoS) là một thuật toán đồng thuận được đề xuất bởi Daniel Larimer (Co-founder EOS). DPoS là sự kết hợp giữa PoA, PoS và hệ thống bỏ phiếu quản trị dựa trên số token nắm giữ. Đây cũng là một trong số những thuật toán được sử dụng thịnh hành trong nền tảng blockchain hiện nay.

##  Ưu và nhược điểm của DPoS

### Khả năng mở rộng cao

- Cơ chế hoạt động của DPoS giúp giảm đi đáng kể số node khi tham gia xác thực giao dịch (validators). Thời gian để đạt được đồng thuận trên DPoS chỉ mất vài giây. Chính vì thế, nó giúp cải thiện đáng kể việc xử lý của hệ thống, giải quyết được bài toán về khả năng mở rộng trên blockchain.
- Cơ cấu quản trị rõ ràng
Cơ cấu quản trị rõ ràng của DPoS được thể hiện cụ thể trong việc hạn chế quyền voting ở các validator node. Mô hình này giúp cho việc đưa ra các quyết định quản trị một cách nhanh hơn so với các blockchain sử dụng PoW hay PoS.

- Phí hoạt động thấp
Các blockchain chạy thuật toán DPoS không cần sở hữu nhiều validator node, yêu cầu cấu hình máy tính cũng không cần mạnh, delegators cũng không cần phải bật máy tính 100%. Vì vậy, năng lượng tiêu thụ bởi việc chạy các blockchain được giảm đi đáng kể. Phí hoạt động cũng sẽ nhỏ hơn so với các blockchain sử dụng thuật toán PoW hay PoS.

### Nhược điểm

- Trên DPoS số lượng node được giới hạn từ 10 - 100 node, nên việc lựa chọn các node sẽ kỹ càng hơn. Việc xác minh giao dịch sẽ thường do người nắm giữ phần lớn quyền lực quyết định. Họ sẽ chia sẻ các phần thưởng khi tham gia vào sản xuất block mới.
- Sự phát triển này có thể giúp có được hai khía cạnh là bảo mật và khả năng mở rộng cao. Nhưng về điểm hạn chế đó là còn tập trung quá nhiều quyền lực vào số lượng nhỏ validator node. Các node sẽ thông đồng với nhau và chi phối luôn cả mạng lưới hoạt động của blockchain này.


# So sánh Proof of Work (PoW) và DPoS
Khi so sánh DPoS với một thuật toán đồng thuận đầu tiên được ra đời trong thị trường Crypto đó là Proof of Work (PoW), thì DPoS đã tìm ra cách để có thể cải thiện điểm yếu của PoW. Đó chính là việc cải thiện được quá trình tạo khối mới ở trong blockchain.

Điểm nâng cấp này đã giúp cho quá trình giao dịch của các hệ thống khi sử dụng thuật toán này sẽ xử lý được nhiều giao dịch hơn với tốc độ nhanh hơn. Nhưng khi so sánh về độ bảo mật, thì PoW vẫn là một thuật toán có độ bảo mật bậc nhất trong các thuật toán đã được ra đời.

## So sánh PoS và DPoS
- Proof of Stake (PoS)
Proof of Stake (PoS) là một cấu trúc đồng thuận, tương tự PoW, nhưng thay vì đòi hỏi công việc hoặc quyền lực tính toán, nó đòi hỏi người thợ phải giữ được một lượng lớn cryptocurrency.

- Ví dụ: cryptocurrency “Stakeproofcoin (SPC)” dựa vào PoS, và Bob sở hữu 2% tất cả SPC tồn tại. Điều này có nghĩa là xác suất khai thác mỏ của Bob bằng khối lượng chứng cứ là 2%.

- PoS có mục đích ngăn chặn các cuộc tấn công bằng cách yêu cầu cao và hạ thấp ưu đãi đáng kể. Để Bob có thể tấn công SPC, anh ấy cần sở hữu phần lớn tất cả token của SPC, điều này yêu cầu rất nhiều tiền ở nơi đầu tiên.

- Ngoài ra, động lực tấn công của anh ta là tương đối thấp, bởi khi anh ta bắt đầu tấn công SPC, anh ấy phải đón nhận rất nhiều từ chính những cú tấn công của anh ta.



- Delegated Proof of Stake (DPoS) là một cấu trúc đồng thuận mới hơn, nó tương tự như PoS nhưng có các tính năng “dân chủ” khác. Một số người cho rằng DPoS hiệu quả và công bằng hơn.

- Người sử dụng của một phiếu bầu mật mã DPoS cho các đại biểu để phục vụ trên một bảng điều khiển của nhân chứng. Rất nhiều biến trong mạng lưới như kích cỡ hay phí giao dịch được kiểm soát bởi bảng điều khiển này.

- Hội đồng nhân chứng cũng chọn các nhân chứng để làm chứng hoặc xác nhận khối. Mạng lưới và người dùng đặt niềm tin vào những nhân chứng được bầu này để cung cấp cho họ những quyền hạn đó, tuy nhiên nếu không hoạt động, họ có thể dễ dàng bị bỏ phiếu ra khỏi “bảng điều khiển của nhân chứng”. Do đó, họ không có động cơ để làm việc xấu đối với cử tri của mình.

- Để thêm vào phần “chứng minh phần đóng góp” của DPoS, các bên liên quan có ảnh hưởng tỷ lệ thuận với số cổ phần của họ trong hệ thống. DPoS được tìm thấy là phân cấp hơn các hệ thống thống nhất khác bởi vì ngưỡng nhập cảnh rất thấp.