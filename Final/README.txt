Bài 1: 
   - Đường link: https://colab.research.google.com/drive/11k1k_hV6kibCpNnbXL5X3NYoPCtErzPE?fbclid=IwAR3C7YuGMnAeH0DEy2MY70n_qVH4-meLs7xd8Nmhtor90ew9ttrfSlcWNpQ
   - Mô tả:
	+ Mô tả dữ liệu: Payment_data là tập dữ liệu tổng hợp về các giao dịch tiền di động. Mỗi bước đại diện cho một giờ mô phỏng. 
	Tập dữ liệu này được thu nhỏ 1/4 so với tập dữ liệu ban đầu được trình bày trong bài báo "Payment: Một trình mô phỏng tiền di động tài chính để phát hiện gian lận".
	Các trường dữ liệu bao gồm:
		. Step: Lập bản đồ đơn vị thời gian trong thế giới thực. Trong trường hợp này, 1 bước là 1 giờ thời gian.
		. Type: TIỀN VÀO, XUẤT KHẨU, NỢ, THANH TOÁN và CHUYỂN KHOẢN.
		. amount: số tiền giao dịch là đơn vị tiền quốc nội.
		. nameOrig: khách hàng - những người đã thực hiện giao dịch
		. oldbalanceOrg: số dư ban đầu trước khi giao dịch.
		. newbalanceOrig: số dư của khách hàng sau khi giao dịch.
		. nameDest: ID người nhận giao dịch.
		. oldbalanceDest: số dư ban đầu của người nhận trước khi giao dịch.
		. newbalanceDest: số dư của người nhận sau khi giao dịch.
		. isFraud: xác định một giao dịch gian lận (1) và không gian lận (0).

	+ Mục tiêu bài toán: phân tích là kiểm tra các dữ liệu về các giao dịch được thực hiện trong một ngân hàng có phải là giao dịch gian lận hay không 
	+ Giải thuật: thay vì load lại toàn bộ data về lịch sử giao dịch thì sẽ chia thành các luồng dữ liệu riêng biệt, các file dữ liệu riêng biệt gồm có: 
	Step tương ứng với id người giao dịch, số lần giao dịch với mỗi id, sử dụng "maxFilesPerTrigger" ghi kết quả đầu ra vào bộ nhớ.


Bài 2:
   - Đường link: https://colab.research.google.com/drive/1g931P3jNyaXwQJqVCzllvu7yjSa_N7jZ?authuser=4#scrollTo=onHv4CNY5rEk
   - Mô tả:
	+ Mô tả dữ liệu: dữ liệu là thu thập các request gửi từ 1 host đến endpoint trong các ngày của tháng. Trong đó, có các trường dữ liệu:
		. Host: phía gửi.
		. Timestamp: thời gian gửi.
		. Method: phương thức gửi request (GET, POST, DELETE, PUT,....).
		. Endpoint: phía nhận.
		. Status: trạng thái của request (200, 404, 401, 408, ....).
		. Content_size: size của request được gửi đi.

	+ Mục tiêu bài toán: Đọc logfile, phân tích dữ liệu trong file đó, trực quan hóa các phân tích bằng sơ đồ


Link video báo cáo:
	- File tổng hợp: https://drive.google.com/file/d/1qI3VNLj_ZBIF3OTz0LwjNuCd6GPS5xnv/view
	- File lý thuyết: https://drive.google.com/file/d/13sqz7pB3_uojlPN2z4KfcEeLS9r1T1CM/view
	- File Bài 1: https://drive.google.com/file/d/13ZiSolt1KJh_Uq_rDx_QuthE9e9CV4EP/view
	- File Bài 2: https://drive.google.com/file/d/1FGsJroKIastCS_Dn-83nBnHrveLENuHE/view
