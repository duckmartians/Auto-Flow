[![Download Here](https://img.shields.io/badge/⬇_Download-Here-success?style=for-the-badge)](https://chromewebstore.google.com/detail/auto-flow-prompt-automati/lhcmnhdbddgagibbbgppakocflbnknoa)

# 🎬 Auto Flow v7.5.5 - Automation for Google VEO AI [![Tiếng Việt](https://img.shields.io/badge/Tiếng%20Việt-green)](README_vi.md) [![English](https://img.shields.io/badge/English-blue)](README.md) 

**Auto Flow** là tiện ích mở rộng (Extension) mạnh mẽ giúp tự động hóa quy trình sáng tạo video trên Google Flow (VEO). Công cụ giúp bạn "treo máy" để tạo hàng trăm video từ văn bản hoặc hình ảnh mà không cần thao tác thủ công lặp đi lặp lại.

[](https://chromewebstore.google.com/detail/auto-flow-automation-for/lhcmnhdbddgagibbbgppakocflbnknoa) [](https://duckmartians.info)

-----

## ✨ Tính năng chính

  * **🚀 Hàng chờ thông minh (Smart Queue):** Thêm hàng loạt prompt hoặc ảnh vào danh sách chờ. Tool sẽ tự động xử lý từng tác vụ một.
  * **📝 Text-to-Video:** Hỗ trợ nhập file `.txt` chứa hàng trăm prompt.
  * **🖼️ Image-to-Video:** Tự động upload ảnh, crop tỷ lệ và tạo chuyển động.
  * **💾 Tự động tải xuống:** Tự động lưu video về máy ngay khi render xong. Hỗ trợ phân loại thư mục theo tên dự án.
  * **🛡️ Cơ chế Retry:** Tự động thử lại khi gặp lỗi mạng hoặc khi hàng chờ của Google bị đầy (Queue Full).
  * **⚙️ Tùy chỉnh sâu:**
      * Chọn Model (Veo 2, Veo 3.1...).
      * Tỷ lệ khung hình (16:9, 9:16).
      * Số lượng video sinh ra cho mỗi prompt (1-4 variants).

-----

## 📥 Cài đặt

1.  Truy cập [Auto Flow trên Chrome Web Store](https://chromewebstore.google.com/detail/auto-flow-automation-for/lhcmnhdbddgagibbbgppakocflbnknoa).
2.  Nhấn **Thêm vào Chrome (Add to Chrome)**.
3.  Truy cập trang [Google Flow](https://labs.google/fx/tools/flow).
4.  Mở Side Panel của Chrome (biểu tượng bên phải thanh địa chỉ) và chọn **Auto Flow**.

-----

## 📖 Hướng dẫn sử dụng

### 1\. Chế độ Text-to-Video

1.  Chọn chế độ **Text-to-Video** ở tab Điều khiển.
2.  Nhập prompt vào ô trống (mỗi prompt cách nhau 1 dòng trắng) HOẶC nhấn nút **Import file (.txt)** để tải lên danh sách prompt.
3.  Cài đặt số lượng video và tỷ lệ khung hình.
4.  Nhấn **Thêm vào hàng chờ** -\> **Bắt đầu Hàng chờ**.

### 2\. Chế độ Image-to-Video

1.  Chọn chế độ **Image-to-Video**.
2.  Nhấn **Chọn ảnh** để tải lên (hỗ trợ chọn nhiều ảnh cùng lúc).
3.  Nhập prompt.
4.  Nhấn **Thêm vào hàng chờ** -\> **Bắt đầu Hàng chờ**.

### 3\. Quản lý Hàng chờ (Queue)

  * Nhấn nút **Quản lý (Manage)** để xem danh sách các tác vụ đang chờ.
  * Bạn có thể **Xóa** tác vụ thừa hoặc **Reset** các tác vụ bị lỗi (Failed) để chạy lại.

-----

## 🔧 Khắc phục sự cố thường gặp

| Vấn đề | Nguyên nhân & Cách xử lý |
| :--- | :--- |
| **Báo lỗi "Queue Full"** | Google Flow giới hạn số lượng video xử lý cùng lúc. **Đừng lo**, Extension sẽ tự động chờ và thử lại sau mỗi 30s cho đến khi slot trống. |
| **Video không tự tải** | Vào Cài đặt Chrome -\> Tệp đã tải xuống -\> **Tắt** mục *"Hỏi vị trí lưu từng tệp"*. |
| **Báo lỗi "Policy Error"** | Prompt hoặc Hình ảnh của bạn vi phạm chính sách nội dung của Google. Tool sẽ tự động bỏ qua tác vụ này và chạy tác vụ tiếp theo. |
| **Màn hình bị Zoom nhỏ** | Đây là tính năng tự động của Tool để bao quát giao diện và tìm nút bấm chính xác hơn. Vui lòng không chỉnh lại zoom khi tool đang chạy. |

-----

## 🔒 Quyền riêng tư & Dữ liệu

  * **Hoạt động cục bộ:** Auto Flow chạy hoàn toàn trên trình duyệt của bạn.
  * **Không thu thập dữ liệu:** Chúng tôi không thu thập prompt, hình ảnh hay video của bạn. Mọi dữ liệu chỉ được lưu tại `Chrome Local Storage` của chính bạn để ghi nhớ cài đặt.
  * **Quyền truy cập:** Extension chỉ yêu cầu quyền truy cập vào trang `labs.google/*` để thực hiện các thao tác tự động hóa.

-----

## ☕ Hỗ trợ tác giả

Phần mềm được phát triển và duy trì miễn phí. Nếu công cụ này giúp bạn tiết kiệm thời gian và nâng cao hiệu suất công việc, hãy cân nhắc mời tác giả một ly cà phê nhé\! ❤️

[duckmartians.info](https://duckmartians.info)

-----

## 📜 Giấy phép (License)

Copyright © 2025 **Đặng Minh Đức (duckmartians)**. All Rights Reserved.

Phần mềm này là tài sản độc quyền. Nghiêm cấm các hành vi sao chép, sửa đổi, phân phối lại mã nguồn hoặc bán lại dưới mọi hình thức mà không có sự cho phép bằng văn bản của tác giả.

-----

*Disclaimer: This extension is an independent project and is not affiliated with, endorsed by, or connected to Google or the Google Flow team.*
