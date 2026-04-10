# MÔN HỌC: HỆ QUẢN TRỊ CƠ SỞ DỮ LIỆU - ThS.ĐỖ DUY CỐP
## Họ và tên: Trần Nhất Nam
## MSSV: K235480106001
## Lớp: K59KMT
# 1. Download và cài đặt SQL Server 2025, phiên bản Developer với 2 kiểu login
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/26f6744c-e645-4ce4-8831-056c6fe1ec37" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ff37a0ac-82f0-4d5e-b1c9-0ada4743d532" />

# 2. Cấu hình cho SQL Server làm việc ở cổng động (Dynamic Port với xxxx=6001)
+ TCP/IP: Enable
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6686eeb9-f587-4751-848e-54f0e44f5259" />

+ Thiết lập TCP Dynamic Ports: 36001
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d6bccbd9-0a69-4170-ac2b-bc4c59fa6d9f" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e55cf08f-4add-4b6f-baec-52f73c7bb795" />

# 3. Tiến hành kiểm tra service SQL Server có đang running và mở đúng cổng đã chọn hay không
<img width="1920" height="1078" alt="image" src="https://github.com/user-attachments/assets/9672d8a0-1b05-4a0b-9e23-cdcf3e7f7774" />

# 4. Cài đặt SQL Server Management Studio
+ Giao diện phần mềm SQL Server Managemnent Studio 22
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/084b9769-246e-48ba-9381-fb2331ffe7c7" />

# 5. Chạy phần mềm SSMS để đăng nhập vào SQL Server bằng 2 cách: Windows Authentication và SQL Server Authentication
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b03b1a2a-8ef1-4005-96e9-41780a61c388" />

# 6. Sử dụng giao diện đồ hoạ của ssms: Tạo cơ sở dữ liệu mới với tên tuỳ ý, lưu tại ổ E
+ Tên cơ sở dữ liệu (Database): SV_6001
+ Vị trí lưu: E:\SQL_Thay_Cop
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/121cc95d-3157-4bee-9b6e-0955c4ade635" />

# 7. Sử dụng giao diện đồ hoạ của SSMS tạo bảng dữ liệu với tên bảng tuỳ ý, có các trường dữ liệu phù hợp với dữ liệu của file data mẫu, với Khoá chính (Primary Key) là trường masv
+ Tạo bảng dữ liệu với tên: Data_SV
+ Khóa chính (Primary Key): masv
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c10238eb-8066-49e0-b929-27d3345f4bf3" />

# 8. Sử dụng giao diện đồ hoạ của SSMS: Tìm cách import dữ liệu từ file mẫu vào trong bảng vừa tạo.
+ Import dữ liệu từ file svtnut.csv thành công
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6aa109cc-5e38-4cc1-a07f-1930ac223743" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e2d488bd-022b-4caa-9b3f-32b66b392d69" />

# 9. Mở cửa sổ mới để gõ lệnh trong SSMS: Gõ lệnh để kiểm tra số dòng của bảng dữ liệu sau khi import, kết quả ok sẽ khoảng 12020 dòng
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/77fbdd9e-e35e-4555-ba69-8e7b926ad840" />

+ Kết quả đúng như yêu cầu của đầu bài, bảng chứa 12020 dòng thông tin của sinh viên
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/90adb475-38db-4fbd-8511-98ea5403a209" />

# 10. Trong cửa sổ mới để gõ lệnh: Gõ lệnh để thêm 1 row vào bảng, với dữ liệu là thông tin cá nhân sinh viên
+ Thông tin sẽ chèn thêm vào bảng: K235480106001,Trần Nhất Nam, K59KMT,31/10/2005,Thái Nguyên,Tổ Cầu - Bách Quang - Thái Nguyên
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dceb8960-c228-46a2-b0c4-67b6964a2aba" />

# 11. Trong cửa sổ mới để gõ lệnh: Gõ lệnh để cập nhật trường noisinh thành 'Sao Hoả' cho những dòng có noisinh và diachi đều là NULL
+ "noisinh" được đổi thành "Sao Hỏa" tại tất cả các dòng có noisinh và diachi là NULL
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7036c3a1-19f4-4905-a26a-11ccc485850c" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/49291ced-2182-4694-a3b9-e016a5000886" />

# 12. Sử dụng giao diện đồ hoạ của ssms: Tạo bảng SaoHoa gồm những sinh viên có nơi sinh ở 'Sao Hoả'
+ Tạo bảng "SaoHoa" thành công, 1438 sinh viên sinh tại Sao Hỏaa
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/193b6994-91fa-4da8-a16c-5c36e230a122" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/12f5838d-0e90-49a8-9e60-3cad17d31c3c" />

# 13. Trong cửa sổ mới để gõ lệnh: Gõ lệnh xoá trong bảng SaoHoa những sinh viên họ Trần
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5f5e91a3-8eed-4c3c-8e14-b562fb3160d9" />

+ Xoá thành công, còn lại 1319 sinh viên sinh ra tại sao Hỏa 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/780ee0e4-3421-4e66-bd8d-d39c75aa726e" />

# 14. Sử dụng giao diện đồ hoạ của SSMS: Xuất toàn bộ kết quả của các bước 6,7,8,9,10,11,12,13 ra file dulieu.sql
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3da24efd-5d3f-4a1b-93b2-dfabe9edab13" />

# 15. Sử dụng giao diện đồ hoạ của SSMS: Xoá csdl đã tạo, sau khi xoá, kiểm tra tại path (path chọn ở bước 6) xem còn tồn tại 2 file của bước 6 không?
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c5f735fe-c58f-4428-9e47-8e31eba0f104" />

+ Database SV_6001 đã bị xóa hoàn toàn
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cf7f8a78-55ef-4e6a-90ad-f7409d32e4aa" />

# 16. Tạo cửa sổ mới để gõ lệnh: mở file dulieu.sql của bước 14, chạy toàn bộ các lệnh này. REFRESH lại cây liệt kê các database => kiểm chứng kết quả được tạo ra tương đương với các bước 6,7,8,9,10,11,12,13.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/52c0efc5-dda7-4bf3-84ff-1f026b2576a1" />

+ Execute code file dulieu.sql thành công
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/474283b7-780c-43c9-a58f-85756f2852d6" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d223c01b-7bf1-4b5b-a00a-e8234ec3a858" />

# 17. File dulieu.sql
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7e6763be-7f70-44ba-8a3f-7bbf3ed1ce7e" />





















