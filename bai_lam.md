# BÀI LÀM – HACKATHON 02

- **Mã đề:** 01
- **Họ tên:** Huỳnh Kế Minh Quân
- **Lớp:** HCM_KS26_CNTT1
- **Link repository:**
- **Hệ điều hành (Windows/macOS):** Windows

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
ls 
ls -Force
 mv .\ghi_chu_ban_giao.txt .\docs\
 mkdir backup
  cp .\data\ban_ve_thang_1.xlsx .\backup\
   rm .\temp_101.tmp
 Get-ChildItem .\logs\
  Get-ChildItem -Recurse -Force
   

```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
  Directory: C:\Users\HP\Downloads\starter-kit\ho-boi-website\ho-boi-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        11/11/2026   8:20 AM                backup
d-----        11/11/2026   8:12 AM                data
d-----        11/11/2026   8:15 AM                docs
d-----        11/11/2026   7:56 AM                evidence
d-----        11/11/2026   8:13 AM                logs
d-----        11/11/2026   7:50 AM                web
------         11/3/2026   7:06 AM             74 .env
-a----         11/3/2026   7:06 AM           2407 bai_lam.md
-a----         11/3/2026   7:06 AM           6106 ban_ve_thang_1.xlsx


    Directory: C:\Users\HP\Downloads\starter-kit\ho-boi-website\ho-boi-website\backup


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         11/3/2026   7:06 AM           6106 ban_ve_thang_1.xlsx


    Directory: C:\Users\HP\Downloads\starter-kit\ho-boi-website\ho-boi-website\data


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         11/3/2026   7:06 AM           6106 ban_ve_thang_1.xlsx


    Directory: C:\Users\HP\Downloads\starter-kit\ho-boi-website\ho-boi-website\docs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         11/3/2026   7:06 AM            158 ghi_chu_ban_giao.txt


    Directory: C:\Users\HP\Downloads\starter-kit\ho-boi-website\ho-boi-website\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         11/3/2026   7:06 AM            972 visit.log


    Directory: C:\Users\HP\Downloads\starter-kit\ho-boi-website\ho-boi-website\web


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        11/11/2026   7:50 AM                images
------         11/3/2026   7:06 AM            574 app.js
------         11/3/2026   7:06 AM            507 index.html
------         11/3/2026   7:06 AM            460 style.css


    Directory: C:\Users\HP\Downloads\starter-kit\ho-boi-website\ho-boi-website\web\images


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
------         11/3/2026   7:06 AM           3061 logo-aquazone.png

```

## 4.3. Lọc log truy cập website

### a) Lệnh lọc các dòng status=500

```shell
Get-Content .\logs\access.log | Select-String "status=500" | ForEach-Object { $_.Line } | Set-Content .\logs\loi_500.txt

```

### 2 dòng đầu tiên trong logs/loi_500.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

### b) Lệnh đếm số dòng status=404 và kết quả

```shell
Get-Content .\logs\access.log | Select-String "status=404" | Measure-Object


```

```text
(Dán kết quả đếm vào đây – xoá dòng này)

```

## 4.4. Chạy script tong_hop (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### Nội dung file logs/tong_hop.txt

```text
(Dán nội dung file vào đây – xoá dòng này)

```

## 4.5. README.md và bảo vệ thông tin bí mật

> README.md, .gitignore và .env.example được chấm trực tiếp trên file ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [ ] README.md: Heading 1, mô tả có **in đậm** và *in nghiêng*, bảng, code block, task list, blockquote
- [ ] .gitignore có dòng `.env` (tên file đúng, không có đuôi .txt)
- [ ] .env.example có đủ tên biến, giá trị để trống (tên file đúng, không có đuôi .txt)

## 4.6. Kiểm tra trang web bằng DevTools (F12) và báo cáo lỗi

### Bảng lỗi

| STT | Tab DevTools phát hiện lỗi | Tên file hoặc thông báo lỗi | Cách khắc phục |
| --- | --- | --- | --- |
| 1 |  |  |  |
| 2 |  |  |  |

> Ảnh chụp màn hình lưu trong thư mục `evidence/` (network.png, console.png).

### Báo cáo lỗi gửi trưởng nhóm

- **Context:** 
- **Expected:** 
- **Actual:** 
- **Log:** 

### Câu tìm kiếm Google

```text
(Ghi câu tìm kiếm vào đây – xoá dòng này)

```

## 4.7. Excel

> Phần Excel được chấm trực tiếp trên file `data/ban_ve_thang_1.xlsx`, không cần ghi vào đây.
