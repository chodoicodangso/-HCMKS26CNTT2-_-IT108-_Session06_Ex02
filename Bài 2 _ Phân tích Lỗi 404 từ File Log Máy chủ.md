**Sai lầm của An là dùng lệnh tìm tên file thay vì tìm nội dung bên trong file.** Lệnh **Get-ChildItem** không thể đọc dữ liệu bên trong tệp tin, dẫn đến kết quả trống rỗng.  
1\. Phân biệt câu lệnh  
**Get-ChildItem:** Tìm kiếm và liệt kê **tên file, thư mục**.  
**Select-String:** Tìm kiếm văn bản **bên trong nội dung** file.  
2\. Câu lệnh đúng   
Select-String \-Path ".\\access.log" \-Pattern "ERROR"

