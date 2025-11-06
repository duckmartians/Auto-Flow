# Hướng dẫn sử dụng Auto Flow

## 1. Giới thiệu

**Auto Flow** là một tiện ích mở rộng (extension) cho trình duyệt Chrome, được thiết kế để tự động hóa quy trình tạo video hàng loạt trên nền tảng Google Flow.

Tiện ích này giúp bạn tiết kiệm thời gian bằng cách tự động gửi hàng loạt các yêu cầu (prompt) hoặc hình ảnh để tạo video, hỗ trợ các model mới nhất như VEO (Veo 2, Veo 3.1) và tự động tải về kết quả.

## 2. Cài đặt & Yêu cầu

### Yêu cầu bắt buộc
1.  **Trang Google Flow:** Tiện ích này **chỉ hoạt động** khi bạn đang mở một trang project trên Google Flow (ví dụ: `https://labs.google/fx/tools/flow/project/...`). Nếu bạn mở ở trang khác, tiện ích sẽ hiển thị thông báo và cung cấp nút để điều hướng đến Flow.
2.  **Cấu hình Tải về (Rất quan trọng):** Để tính năng "Tự động tải video" hoạt động mượt mà, bạn **phải** tắt cài đặt "Hỏi vị trí lưu..." trong trình duyệt.
    * Mở Cài đặt của Chrome: `chrome://settings/downloads`
    * Tắt tùy chọn: **Hỏi vị trí lưu mỗi tệp trước khi tải xuống** (Ask where to save each file before downloading).
    * Bạn cũng có thể nhấp vào liên kết "Cấu hình thư mục" trong Tab Cài Đặt của extension để mở nhanh trang này.

## 3. Hướng dẫn sử dụng chi tiết

Giao diện của Auto Flow được chia làm 4 tab chính.

### 3.1. Tab "Điều Khiển" (Control)

Đây là nơi bạn thiết lập và bắt đầu quá trình tự động hóa.

#### Bước 1: Chọn Chế độ (Creation Mode)

Bạn có hai chế độ để tạo video:

* **Text-to-Video:**
    * **Mục đích:** Tạo video hàng loạt chỉ từ danh sách các câu lệnh (prompt).
    * **Cách dùng:** Chọn chế độ này và chuyển đến Bước 2.
* **Image-to-Video:**
    * **Mục đích:** Tạo video hàng loạt bằng cách kết hợp một danh sách ảnh và một danh sách prompt.
    * **Cách dùng:**
        1.  Nhấn nút **"Chọn ảnh (nhiều ảnh)"** để tải lên các file ảnh của bạn.
        2.  Sử dụng menu thả xuống **"Sắp xếp ảnh"** để chọn thứ tự xử lý ảnh (A-Z, Z-A, Mới nhất, Cũ nhất).
        3.  Chuyển đến Bước 2 để nhập prompt. Các prompt này sẽ được sử dụng tuần hoàn cho danh sách ảnh của bạn (ví dụ: 5 ảnh và 2 prompt, thì ảnh 1, 3, 5 dùng prompt 1; ảnh 2, 4 dùng prompt 2).

#### Bước 2: Nhập Dữ liệu (Prompt/Ảnh)

* **Nhập Prompt:**
    * **Gõ trực tiếp:** Gõ các prompt của bạn vào ô "Danh sách prompt". **Quan trọng:** Mỗi prompt phải được **cách nhau bằng ít nhất MỘT DÒNG TRỐNG** (nhấn Enter 2 lần).
    * **Nhập từ file:** Nhấn nút **"Nhập từ file (.txt)"** để tải lên một file văn bản. Các prompt trong file cũng phải được cách nhau bằng dòng trống.
* **Nhập Ảnh:** (Chỉ cho chế độ Image-to-Video) Đã hoàn thành ở Bước 1.

#### Bước 3: Bắt đầu chạy (Start)

Nhấn nút **"Bắt đầu"** (Start). Bạn sẽ thấy hai lựa chọn:

1.  **🚀 Tạo dự án mới (Create New Project):**
    * Tool sẽ tự động điều hướng đến trang chủ Flow, tạo một project mới, sau đó bắt đầu chạy các tác vụ của bạn trên project đó.
    * *Nên dùng khi bạn muốn bắt đầu một lô công việc mới hoàn toàn.*
2.  **➡️ Chạy luôn tại đây (Run on This Page):**
    * Tool sẽ chạy ngay lập tức trên project bạn đang mở.
    * *Nên dùng khi bạn muốn tiếp tục công việc trên một project có sẵn.*

#### Các nút điều khiển khác:

* **Tạm dừng / Tiếp tục (Pause / Continue):** Khi đang chạy, nút "Bắt đầu" sẽ chuyển thành nút "Tạm dừng". Nhấn để tạm ngưng, và nhấn lại ("Tiếp tục") để chạy tiếp từ vị trí đã dừng.
* **Dừng (Stop):** Nhấn nút này để hủy bỏ hoàn toàn quy trình đang chạy.

### 3.2. Tab "Cài Đặt" (Settings)

Tinh chỉnh các thông số để phù hợp với nhu cầu của bạn.

* **Số lượng video mỗi tác vụ:** Chọn số lượng video (1-4) mà Flow sẽ tạo ra cho MỖI prompt hoặc MỖI ảnh.
* **Bắt đầu từ (Prompt/Ảnh):** Nhập số thứ tự của tác vụ bạn muốn bắt đầu. Ví dụ: nếu bạn có 100 prompt và muốn bắt đầu từ prompt thứ 50, hãy nhập `50`.
* **Thời gian chờ tạo video (giây):** Đặt khoảng thời gian chờ (tối thiểu - tối đa) sau khi gửi mỗi tác vụ. Tool sẽ chọn ngẫu nhiên một con số trong khoảng này để chờ video tạo xong trước khi gửi tác vụ tiếp theo.
* **Model (Tùy chọn):** Chọn model VEO bạn muốn sử dụng (Fast hoặc Quality). "Mặc định" thường là Veo 3.1 - Fast.
* **Tỷ lệ (T2V & I2V Crop):** Chọn tỷ lệ khung hình (Ngang 16:9 hoặc Dọc 9:16).
* **Ngôn ngữ (Language):** Đổi ngôn ngữ giao diện của tiện ích (Tiếng Việt / English).
* **Tự động tải video:**
    * Khi được bật, tool sẽ tự động quét và tải về các video ngay khi chúng được tạo xong.
    * **Lưu ý:** Tính năng này yêu cầu bạn phải tắt "Hỏi vị trí lưu..." trong cài đặt trình duyệt (xem mục 2. Cài đặt & Yêu cầu).

### 3.3. Tab "Lịch Sử" (History)

Theo dõi và gỡ lỗi quy trình của bạn.

* **Log chi tiết:** Hiển thị chi tiết từng bước mà tool đang thực hiện (đã gửi tác vụ, đang chờ, đã tải video, lỗi...).
* **Tác vụ lỗi:** Liệt kê tất cả các prompt hoặc tên ảnh bị thất bại (ví dụ: do lỗi chính sách của Google, lỗi mạng, hoặc tool không thể xử lý).
    * Tool sẽ tự động thử lại một tác vụ tối đa 5 lần trước khi đánh dấu là lỗi.
* **Sao chép các prompt/ảnh lỗi:** Nhấn nút này để sao chép toàn bộ danh sách các tác vụ lỗi vào clipboard. Bạn có thể dán danh sách này vào một file `.txt` mới hoặc dán trực tiếp vào ô prompt để chạy lại sau.

### 3.4. Tab "Tools Khác" (More Tools)

Khám phá các tiện ích hữu ích khác từ tác giả.

---

## 4. Mẹo và Lưu ý

* **Lỗi Chính sách (Policy Error):** Nếu Google Flow báo lỗi chính sách (policy error) cho một prompt hoặc ảnh, tool sẽ tự động phát hiện, ghi lại trong tab Lịch Sử và bỏ qua tác vụ đó để tiếp tục chạy.
* **Giữ Tab Mở:** Luôn giữ tab Google Flow (nơi tool đang chạy) được mở và hiển thị để đảm bảo hoạt động ổn định.
* **Chờ đợi:** Nếu bạn có danh sách hàng trăm tác vụ, hãy kiên nhẫn. Tool cần thời gian để xử lý và chờ Google Flow tạo video.
