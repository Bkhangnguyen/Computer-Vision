# So sánh PIL và OpenCV trong xử lý ảnh

## Cơ bản 

* PIL (Pillow) : Thư viện xử lý ảnh mức cơ bản, cú pháp đơn giản, thích hợp cho người nhập môn.

* OpenCV (cv2) : Thư viện mạnh mẽ, hiệu năng cao, dùng cho thị giác máy tính ở mức chuyên sâu.

## So sánh khái niệm  

Tiêu chí :

* PIL : 

        - Dễ học dễ sử dụng , áp dụng đơn giản .

        - Hiệu năng của PIL ở ngưỡng trung bình, chạy đủ nhanh cho các tác vụ đơn giản, nhưng không tối ưu cho xử lý nặng hoặc số lượng lớn ảnh.

        - PIL dùng cho học tập và các tác vụ đơn giản .

* OpenCV : 

        - Khó học hơn PIL do cú pháp và khái niệm phức tạp hơn, hướng tới người dùng có kiến thức nền về xử lý ảnh.

        - Hiệu năng cao: xử lý nhanh, tối ưu tài nguyên, tận dụng tốt NumPy, CPU đa nhân và có thể mở rộng với GPU.

        - Phù hợp cho bài toán lớn, ảnh độ phân giải cao, xử lý video hoặc thời gian thực.

## Kết luận khái niệm cơ bản :

* Chọn **PIL** nếu cần xử lý ảnh đơn giản, nhanh gọn.
* Chọn **OpenCV** nếu cần hiệu năng cao và các thuật toán xử lý ảnh nâng cao.

## So sánh chi tiết của 2 bài trên 
1. Sự khác nhau giữa 2 cách làm :

PIL: 2.1.1_Images_with_python_library_PIL.ipynb 

        - Sử dụng thư viện Pillow (PIL).

        - Ảnh được xử lý dưới dạng Image object.

        - Cú pháp mang tính mô tả, gần với cách con người hiểu ảnh (open, show, resize…).

OpenCV: 2.1.2_Images_with_python_library_CV.ipynb

        - Sử dụng thư viện OpenCV (cv2).

        - Ảnh được biểu diễn dưới dạng NumPy array.

        - Cách làm việc mang tính toán học và mảng số, phù hợp cho xử lý nâng cao.

2. Nội dung câu lệnh đọc và hiển thị :

PIL: 2.1.1_Images_with_python_library_PIL.ipynb 
        - Khi đọc dùng : Image.open()
        - Được hiển thị : image show()
        - Định dạng màu sắc : RGB 

OpenCV: 2.1.2_Images_with_python_library_CV.ipynb
        - Khi đọc dùng : cv2.imread()
        - Được hiển thị : cv2.imshow()
        - Định dạng màu sắc : BGR 


3. Các thao tác xử lý ảnh :
PIL: 2.1.1_Images_with_python_library_PIL.ipynb tập trung vào:

    + Mở và hiển thị ảnh.

    + Resize, crop.

    + Chuyển đổi chế độ ảnh (RGB, grayscale).

    + Các thao tác cơ bản, trực quan

OpenCV: 2.1.2_Images_with_python_library_CV.ipynb tập trung vào:

    + Đọc ảnh bằng cv2

    + Chuyển đổi không gian màu

    + Xử lý ảnh bằng NumPy

    + Các thao tác chuẩn bị cho thị giác máy tính

4. Kết luận dựa trên 2 tệp :

Hai notebook có cùng mục tiêu học xử lý ảnh, nhưng
PIL notebook tập trung vào sự đơn giản và trực quan,
trong khi OpenCV notebook tập trung vào hiệu năng và khả năng mở rộng cho thị giác máy tính.



