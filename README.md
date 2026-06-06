# Shutdown

Shutdown là một tiện ích nhỏ gọn dành cho Windows giúp tự động lưu các tài liệu Office đang mở trước khi tắt máy.

Ứng dụng sử dụng COM Automation để kết nối với Microsoft Office, lưu các tài liệu chưa được lưu, đóng Office một cách an toàn, sau đó thực hiện quá trình shutdown của Windows. Điều này giúp giảm nguy cơ mất dữ liệu khi người dùng quên lưu Word, Excel hoặc PowerPoint trước khi tắt máy.

## Tính năng

* Tự động lưu tài liệu Word đang mở.
* Tự động lưu Workbook Excel đang mở.
* Tự động lưu Presentation PowerPoint đang mở.
* Đóng Office sau khi hoàn tất lưu dữ liệu.
* Tự động đóng các ứng dụng giao diện người dùng còn đang chạy.
* Thực hiện shutdown Windows sau khi hoàn tất.
* Chạy hoàn toàn ẩn, không hiển thị cửa sổ PowerShell.
* Biên dịch thành một file EXE duy nhất.
* Không phụ thuộc thư viện MinGW/MSYS2 bên ngoài.

## Yêu cầu

* Windows 10 hoặc Windows 11
* Microsoft Office đã được cài đặt

## Build

Dự án được biên dịch bằng g++ (MSYS2 MinGW64) với liên kết tĩnh (static linking) để tạo ra file thực thi độc lập, dễ dàng sử dụng trên nhiều máy tính mà không cần cài đặt thêm runtime.

## Lưu ý

Tiện ích được thiết kế cho mục đích sử dụng cá nhân nhằm tự động hóa quá trình lưu tài liệu và tắt máy. Người dùng nên kiểm tra kỹ với các tệp Office quan trọng trước khi sử dụng trong môi trường sản xuất.
