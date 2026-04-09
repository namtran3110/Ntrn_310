* Họ và tên: Trần Nhất Nam
* MSSV: K235480106001
* Lớp: K59KMT
# 1. Download và cài đặt SQL Server 2025, phiên bản Developer
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/26f6744c-e645-4ce4-8831-056c6fe1ec37" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ff37a0ac-82f0-4d5e-b1c9-0ada4743d532" />

# 2. Cấu hình cho SQL Server làm việc ở cổng động (Dynamic Port với xxxx=6001)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6686eeb9-f587-4751-848e-54f0e44f5259" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d6bccbd9-0a69-4170-ac2b-bc4c59fa6d9f" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e55cf08f-4add-4b6f-baec-52f73c7bb795" />

# 3. Tiến hành kiểm tra service SQL Server có đang running và mở đúng cổng đã chọn hay không
<img width="1920" height="1078" alt="image" src="https://github.com/user-attachments/assets/9672d8a0-1b05-4a0b-9e23-cdcf3e7f7774" />

# 4. Cài đặt SQL Server Management Studio
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/084b9769-246e-48ba-9381-fb2331ffe7c7" />

# 5. Chạy phần mềm ssms để đăng nhập vào SQL Server bằng 2 cách: Windows Authentication và SQL Server Authentication
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b03b1a2a-8ef1-4005-96e9-41780a61c388" />

# 6. Sử dụng giao diện đồ hoạ của ssms: Tạo cơ sở dữ liệu mới với tên tuỳ ý, lưu tại ổ E
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/121cc95d-3157-4bee-9b6e-0955c4ade635" />

# 7. Sử dụng giao diện đồ hoạ của ssms: Tạo bảng dữ liệu (create and design table) với tên bảng tuỳ ý, có các trường dữ liệu phù hợp với dữ liệu của file data mẫu (CSV), với Khoá chính (Primary Key) là trường masv
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c10238eb-8066-49e0-b929-27d3345f4bf3" />

# 8. Sử dụng giao diện đồ hoạ của ssms: Tìm cách import dữ liệu từ file mẫu vào trong bảng vừa tạo.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c9f1f96b-13f1-4ae9-85fb-1e9b667e9026" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6aa109cc-5e38-4cc1-a07f-1930ac223743" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e2d488bd-022b-4caa-9b3f-32b66b392d69" />

# 9. Mở cửa sổ mới để gõ lệnh trong ssms: GÕ lệnh để kiểm tra xem số dòng của bảng dữ liệu sau khi import, kết quả ok sẽ khoảng 12020 dòng
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/77fbdd9e-e35e-4555-ba69-8e7b926ad840" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/90adb475-38db-4fbd-8511-98ea5403a209" />

# 10. Trong cửa sổ mới để gõ lệnh: Gõ lệnh để thêm (insert) 1 row vào bảng, với dữ liệu là thông tin cá nhân: K235480106001,Trần Nhất Nam, K59KMT,31/10/2005,Thái Nguyên,Tổ Cầu - Bách Quan - Thái Nguyên
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dceb8960-c228-46a2-b0c4-67b6964a2aba" />

# 11. Trong cửa sổ mới để gõ lệnh: Gõ lệnh để cập nhật(update) trường noisinh thành 'Sao Hoả' cho những dòng có noisinh và diachi đều là NULL


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7036c3a1-19f4-4905-a26a-11ccc485850c" />

# 12. 











