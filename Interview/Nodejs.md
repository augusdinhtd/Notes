- Những ưu điểm của nodejs
- Bất đồng bộ với đơn luồng có xung đột gì?
- Scope, protype trong javascript
- tham trị, tham chiếu
- Phân biệt undefined, null, NaN
	Undefined: khi khai báo một biến nhưng chưa gán giá trị cho nó. Khi không khai báo mà log biến đó ra thì trình duyệt báo lỗi biến "is not defined".
	
	Null: Đại diện cho một giá trị không tồn tại, cần gán cho 1 biến.

	NaN: khi function hoặc operation không thể trả về 1 số cụ thể. vd: 0/0, bất kỳ phép tính trong đó NaN là 1 toán hạng,...
	
	typeof undefined -> undefined
	typeof null -> object
	typeof NaN -> number
	null == undefined -> true
	null === undefined -> false

- Tiêu chuẩn call API: REST & SOAP
	REST: GET, POST, PUT, PATH, DELETE, HEAD, OPTIONS
	Sự khác biệt giữa các method update (PUT, PATH)
	- Khi sử dụng PUT: ta phải gửi bản ghi đầy đủ các field để cập nhật, nếu chỉ gửi một số field nhất định thì những field còn lại sẽ bị xóa (tức bị null)
	- PATH: Chỉ thay đổi những field được yêu cầu