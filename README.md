# Top-10-OWASP-2024
<h3>1. Kiểm Soát Truy Cập Bị Phá Vỡ (Broken Access Control)</h3>
<p>Người dùng có thể truy cập hoặc thực hiện hành động không được phép do thiếu kiểm tra quyền hạn hoặc tham chiếu trực tiếp đối tượng không an toàn (IDOR).</p>
<p>Biện pháp: Sử dụng kiểm soát truy cập dựa trên vai trò (RBAC), nguyên tắc quyền tối thiểu, kiểm tra quyền truy cập và sử dụng tham chiếu gián tiếp.</p>
<h3>2. Thất Bại Mã Hóa (Cryptographic Failures)</h3>
<p>Dữ liệu không được mã hóa đúng cách hoặc sử dụng thuật toán lỗi thời như MD5, SHA-1.</p>
<p>Biện pháp: Sử dụng TLS để mã hóa dữ liệu, thuật toán AES-256 cho dữ liệu và bcrypt, scrypt hoặc Argon2 cho mật khẩu.</p>
<h3>3. Lỗ Hổng Tiêm Nhiễm (Injection)</h3>
<p>Xảy ra khi đầu vào của người dùng không được kiểm tra và chèn vào truy vấn SQL hoặc lệnh hệ thống.</p>
<p>Biện pháp: Sử dụng truy vấn tham số hóa, kiểm tra và làm sạch đầu vào.</p>
<h3>4. Thiết Kế Không An Toàn (Insecure Design)</h3>
<p>Lỗ hổng từ giai đoạn thiết kế, như quản lý phiên kém, xử lý lỗi kém, hoặc không có kiểm tra bảo mật.</p>
<p>Biện pháp: Xây dựng mô hình mối đe dọa và kiểm tra bảo mật trong suốt vòng đời ứng dụng.</p>
<h3>5. Cấu Hình Bảo Mật Sai (Security Misconfiguration)</h3>
<p>Sử dụng cấu hình mặc định không an toàn hoặc không vá lỗi hệ thống.</p>
<p>Biện pháp: Thay đổi thông tin đăng nhập mặc định, vá lỗi thường xuyên và kiểm tra bảo mật định kỳ.</p>
<h3>6. Thành Phần Lỗi Thời và Dễ Bị Tấn Công (Vulnerable and Outdated Components)</h3>
<p>Sử dụng thư viện, plugin lỗi thời hoặc không được bảo trì.</p>
<p>Biện pháp: Cập nhật định kỳ các thành phần bên ngoài.</p>
<h3>7. Lỗi Xác Thực và Nhận Diện (Identification and Authentication Failures)</h3>
<p>Mật khẩu yếu, không có xác thực đa yếu tố (MFA), tấn công brute-force.</p>
<p>Biện pháp: Sử dụng MFA, khóa tài khoản sau nhiều lần đăng nhập sai, yêu cầu mật khẩu phức tạp.</p>
<h3>8. Lỗi Toàn Vẹn Phần Mềm và Dữ Liệu (Software and Data Integrity Failures)</h3>
<p>Cập nhật phần mềm không an toàn hoặc không kiểm tra xác thực mã nguồn.</p>
<p>Biện pháp: Sử dụng ký mã và kiểm tra xác thực.</p>
<h3>9. Lỗi Ghi Log và Giám Sát Bảo Mật (Security Logging and Monitoring Failures)</h3>
<p>Không ghi nhận hoặc giám sát các sự kiện bảo mật, làm chậm trễ phát hiện tấn công.</p>
<p>Biện pháp: Xây dựng hệ thống quản lý log và giám sát tập trung.</p>
<h3>10. Giả Mạo Yêu Cầu Phía Máy Chủ (Server-Side Request Forgery - SSRF)</h3>
<p>Cho phép kẻ tấn công gửi yêu cầu từ máy chủ đến tài nguyên không an toàn.</p>
<p>Biện pháp: Kiểm tra và giới hạn đầu vào URL, phân đoạn mạng để bảo vệ tài nguyên nhạy cảm.</p>
