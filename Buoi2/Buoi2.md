# Hash Function 

- Hash Function chuyển đổi các chuỗi có độ dài khác nhau thành các chuỗi có độ dài cố định được gọi là Hash Value (giá trị băm) hoặc tóm tắt, phân loại, sắp xếp có hệ thống. 

- Ý nghĩa của động từ "hash - băm" - cắt hoặc xáo trộn một cái gì đó - cung cấp manh mối về những gì Hash function làm với dữ liệu. Họ "xáo trộn" dữ liệu và chuyển đổi nó thành một giá trị số. Và bất kể đầu vào dài bao nhiêu, giá trị đầu ra luôn có cùng độ dài

# SHA-256

- SHA-256 là một hàm băm không đối xứng (asymmetric hash function), có khả năng chuyển đổi một chuỗi ký tự (message) có độ dài tùy ý thành một chuỗi băm có độ dài cố định là 256 bit (32 byte). Việc tạo ra một chuỗi băm độc nhất cho một chuỗi ký tự cụ thể là rất khó, và đây là lý do tại sao SHA-256 và các thuật toán băm khác được sử dụng rộng rãi trong các ứng dụng bảo mật.
- Các đặc tính của SHA-256 bao gồm tính khó phân tích ngược, tính chống va chạm (collision resistance), tính xác định (deterministic), tính không thể dự đoán được (non-predictive), và tính bảo mật cao. SHA-256 được sử dụng trong nhiều ứng dụng bảo mật như xác thực mật khẩu, chữ ký điện tử, và mã hóa dữ liệu.

# Mã hóa dối xứng và mã hóa không đối xứng

-Mã hóa đối xứng:

- Là lớp thuật toán các mã hóa trong đó việc mã hóa và giải mã đều dùng chung cho 1 khóa (secret key)
-  Mật mã luồng mã hóa từng bit của thông điệp trong khi mật mã khối gộp một số bit lại và mật mã hóa chúng như một đơn vị. Cỡ khối được dùng thường là các khối 64 bit

- Ví dụ: A muốn gửi một tin nhắn cho B.A sẽ mã hóa tin nhắn sau đó gửi cho B.B sẽ giải mã tin nhắn bằng cùng một khóa bí mật và sau đó đọc tin nhắn

#
-Mã hóa bất đối xứng:

- Mã hoá bất đối xứng (hay còn gọi là mã hoá công khai): Có thể hiểu là người ta dùng hai chìa khoá khác nhau để khoá và mở khoá thông tin bí mật. public key sẽ được công khai, và được gửi đi đến đối tượng cần mã hoá thông tin, còn private key được giữ bí mật, và nó đóng vai trò như chìa khoá vạn năng có thể mở được tất cả thông tin được khoá bằng public key.
- Trong blockchain, mã hóa bất đối xứng được sử dụng để xác thực người dùng và đảm bảo tính toàn vẹn của các giao dịch. Khi một người dùng tạo ra một giao dịch mới trên blockchain, họ sẽ tạo chữ ký số (digital signature) bằng cách sử dụng khóa bí mật của mình. Chữ ký số này sẽ được gắn vào giao dịch và chuyển đi trên mạng blockchain cùng với thông tin giao dịch.
- Ví dụ: A gửi tin nhắn cho B mà B đọc được.A sẽ sử dụng khóa của B để mã hóa sau đó tin nhắn mã hóa sẽ được gửi cho B .Sau đó B sẽ mã hóa tin nhắn bằng khóa bí mật để đọc được thông tin 


# Cấu trúc của một Block

-Cấu trúc chung của một block bao gồm:
- Block size: Kích thước của block đó, bao gồm cả các thành phần của nó.
- Block Header: Là phần quan trọng nhất của block, chứa các thông tin về phiên - bản (version) của block, thời gian tạo block (timestamp), Merkle Root, nonce, previous hash và difficult target.
- Transaction data: Là nội dung chính của block, bao gồm tất cả các giao dịch được thực hiện trong mạng.
- Transaction counter: Số lượng giao dịch trong block.


## Block size:
-Kích thước khối khá đơn giản đó là lượng dữ liệu mà một khối có thể chứa.
-Lượng dữ liệu lớn nhất mà một khối blockchain có thể chứa được gọi là giới hạn blocksize

-  Ví dụ: kể từ tháng 5 năm 2021, một khối trên chuỗi khối Bitcoin có thể chứa dữ liệu tương đương 1 MB. Hạn chế này đã được thực thi vào năm 2010, trong nỗ lực hạn chế cơ hội áp đảo chuỗi khối và ngăn chặn các cuộc tấn công DoS có thể xảy ra . 
Ban đầu, chuỗi khối Bitcoin được thiết kế để hoạt động với các khối có kích thước lên tới 36 MB; tuy nhiên, những lo ngại về bảo mật đã buộc phải có kích thước khối nhỏ hơn đáng kể. 

##  Block Header ( version , timestamp , merkle root (giải thích về merkle tree ) , nonce , previous hash , difficult target ) ?

-Version:
- Nó cho biết phiên bản mà khối cụ thể đang sử dụng, có ba loại phiên bản Blockchain.

- Phiên bản chuỗi khối 1.0 (tiền điện tử) - Nó sử dụng sổ cái công khai để lưu trữ dữ liệu, chẳng hạn như Bitcoin.
- Phiên bản chuỗi khối 2.0 (Hợp đồng thông minh) - Nó được gọi là hợp đồng thông minh là các chương trình tự thực hiện, ví dụ như Ethereum.
- Phiên bản chuỗi khối 3.0 (DAPPS) - Nó được sử dụng để tạo cấu trúc phi tập trung, chẳng hạn như trình duyệt tor.
- Phiên bản chuỗi khối 4.0 (Blockchain cho ngành công nghiệp) - Nó được sử dụng để tạo ra một mạng chuỗi khối có thể mở rộng, giá cả phải chăng để nhiều người có thể sử dụng nó hơn.

-timestamp:
- Là một trường (field) trong phần đầu của mỗi block, chứa thời gian tạo block đó. Thời gian này được ghi bằng số giây tính từ thời điểm Unix Epoch (tức là 1/1/1970, 00:00:00 UTC). 

-merkle root:
- Gốc Merkle sử dụng các công thức toán học để kiểm tra xem dữ liệu có bị hỏng, bị tấn công hoặc bị thao túng hay không. 
- Ví dụ: Giả sử một khối có 10 giao dịch, sau đó để xác định khối đó, chúng ta cần 10 giao dịch kết hợp và tạo thành một Giá trị băm, vì vậy nó sử dụng khái niệm cây nhị phân để tạo hàm băm của khối và giá trị đó được gọi là Merkle Gốc

-nonce:

- Nonce là một giá trị ngẫu nhiên được sử dụng để tạo ra một block hợp lệ trong blockchain. Nonce được sử dụng để giải quyết vấn đề khó khăn của bài toán Proof of Work (PoW) trong các hệ thống blockchain.

-previous hash:
- là một giá trị hash được tính toán từ block trước đó trong chuỗi block của blockchain. Nó được lưu trữ trong block header của mỗi block và là một trong những yếu tố quan trọng để kết nối các block lại với nhau trong chuỗi. Điều này đảm bảo rằng mỗi block trong chuỗi sẽ được liên kết với block trước đó và tạo ra một chuỗi liên tiếp của các block, đồng thời giúp đảm bảo tính toàn vẹn của dữ liệu trong blockchain

-difficult target:
- Nó chỉ định độ phức tạp và sức mạnh tính toán cần thiết để khai thác mạng, nếu chúng ta đang gặp mục tiêu có độ khó cao thì điều đó có nghĩa là chúng ta cần nhiều máy tính đắt tiền hơn để khai thác mạng. Ví dụ, để tăng độ khó cho các thuật toán mục tiêu như SHA-2, SHA-3. RIPEMD, MD5,BLAKE2 được sử dụng.

## Transaction data 
-  là thông tin được thu thập từ các giao dịch. Nó ghi lại thời gian giao dịch, địa điểm diễn ra, mức giá của các mặt hàng đã mua, phương thức thanh toán được sử dụng, giảm giá nếu có, số lượng và chất lượng khác liên quan đến giao dịch. Dữ liệu giao dịch thường được thu thập tại điểm bán hàng.
- Nói cách khác, dữ liệu giao dịch là dữ liệu được tạo bởi các ứng dụng khác nhau trong khi chạy hoặc hỗ trợ các quy trình mua và bán hàng ngày của doanh nghiệp. Một trang web lớn và phức tạp gồm các máy chủ điểm bán hàng, phần mềm bảo mật, ATM và dữ liệu cổng thanh toán tồn tại, bắt nguồn từ mọi thiết bị có thể được sử dụng để hoàn tất giao dịch tài chính.
- Với số lượng lớn các điểm tiếp xúc, dữ liệu kết quả thường khó đọc hoặc chứa các phần bổ sung không cần thiết như chữ cái, ký hiệu hoặc số. Việc nắm bắt rõ ràng dữ liệu giao dịch rất hữu ích để chạy các phân tích xuôi dòng, ngăn chặn các cuộc gọi hỗ trợ khách hàng tốn kém hoặc theo dõi sự thật trong các khiếu nại gian lận.

## Transaction Counter

- Trong mạng lưới blockchain, mỗi khối (block) bao gồm nhiều giao dịch (transaction) được thực hiện bởi các người dùng trên mạng. Transaction counter là một trường chỉ ra số lượng giao dịch có trong khối đó. Trường này là một số nguyên không dấu 32-bit và được mã hóa dưới dạng Little-endian.
- Việc theo dõi transaction counter trong các khối là quan trọng để giám sát tốc độ xử lý và đảm bảo tính nhất quán của dữ liệu trên mạng lưới blockchain. Nếu số lượng giao dịch trong khối quá lớn, việc xử lý và truyền tải khối đó sẽ mất nhiều thời gian và tài nguyên hơn. Tuy nhiên, nếu số lượng giao dịch trong khối quá ít, thì việc sử dụng tài nguyên để tạo khối sẽ không được tối ưu.
Transaction Data