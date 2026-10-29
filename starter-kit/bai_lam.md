# BÀI LÀM – THI THỬ HACKATHON 02 (GAMEZONE)

- **Họ tên:** Nguyễn Duy Hưng
- **Lớp:** CNTT 4
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):** 

## 4.2. Thao tác CLI

### Các lệnh đã chạy

```shell
- Hiển thị đường dẫn tuyệt đối thư mục hiện tại: 
        pwd
- Liệt kê nội dung, gồm cả file ẩn: 
        ls
- Di chuyển cap_nhat.txt vào docs, file logo vào media: 
        move cap_nhat.txt docs\ , move logo media\
- Sao chép logo từ media vào backup: 
        copy media\logo backup\
- Xoá file .tmp ở gốc; không xoá file khác:
        Remove-Item .\temp_207.tmp.txt
- Dùng đường dẫn tương đối vào logs, liệt kê nội dung rồi quay lại gốc:
        cd .\logs\  ,  ls  , cd ..
 

```


## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
- Lọc các dòng chứa ERROR trong logs/game.log, ghi vào logs/daily_report.txt:
        Get-Content logs\game.log | Select-String "ERROR" | Set-Content logs\daily_report.txt
- Đọc file báo cáo để kiểm tra; ghi lệnh và dán 2 dòng lỗi đầu tiên vào bai_lam.md:
        Get-Content logs\daily_report.txt -TotalCount 2 

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
(Dán kết quả vào đây)

```

## 4.4. README.md

# Nhập môn công nghệ thông tin

***Ngành sử dụng máy tính, mạng và phần mềm để tự động hóa việc thu thập, xử lý, lưu trữ và truyền tải thông tin số.***

|Trí tuệ nhân tạo | Lập trình web | Lập trình app | An toàn thông tin 
| :--: | :--: | :--: | :--: |
| Chatbot LLM | Frontend React | IOS Swift | Kiểm thử thâm nhập |
| Nhận diện ảnh | Backend Node/Java | Android | Phòng chống mã độc |
| Dự báo số liệu | Sàn TMĐT | Flutter đa nền | Mã hóa dữ liệu |

```PowerShell
    ls
``` 

- [x] Xem elearning.

- [ ] Làm bài tập về nhà.

> không upload .env.

## 4.5. Chạy script auto_report

### Lệnh chạy

```shell
# Ghi lệnh vào đây

```

### Nội dung file logs/auto_report.txt

```text
(Dán kết quả vào đây)

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
- Đếm số dòng chứa ERROR trong logs/game.log bằng pipeline (|). Ghi lệnh và kết quả vào bai_lam.md: 
        (Get-Content .\logs\game.log | Select-String "ERROR").Count

```

### Kết quả đếm

```text
- Kết quả: 6

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
- Dòng đầu tiên: === TONG HOP LOG ===
        "=== TONG HOP LOG GAMEZONE ===" > logs/tong_hop.txt

- Tiếp theo: các dòng chứa WARNING trong logs/web.log
        Get-Content logs/web.log | Select-String "WARNING" >> logs/tong_hop.txt

- Cuối cùng: số dòng chứa ERROR trong logs/web.log.
        (Get-Content logs/web.log | Select-String "ERROR").Count >> logs/tong_hop.txt
```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây)

```

## 4.8. Excel

> Chấm trực tiếp trên file `data/giao_dich_thang_11.xlsx`.
