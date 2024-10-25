# Project: Sales Prediction - dự đoán giá quảng cáo

**Hồi quy tuyến tính - Linear Regression** là mô hình phân tích mối quan hệ phụ thuộc của Y với một hay nhiều biến X sử dụng hàm tuyến tính (hàm đa thức bậc 1). Các tham số của mô hình (hay hàm số) được ước lượng từ dữ liệu huấn luyện.

Dựa vào dữ liệu huấn luyện thông qua phương pháp học gradient descent để tìm bộ tham số tối ưu cho phương trình tuyến tính. Trong mỗi lần học, từ dữ liệu huấn luyện tính toán giá trị dự đoán, sau đó kết hợp với giá trị cần dự đoán trong thực tế để tính toán hàm mất mát (loss), rồi cập nhật lại tham số mô hình dựa vào tính đạo hàm. Quá trình huấn luyện cần chọn lựa các tham số ảnh hưởng đến kết quả của mô hình như tốc độ học (learning rate), giá trị khởi tạo của tham số và số vòng lặp thực hiện cập nhật trọng số.

Tuy nhiên, một nhược điểm của mô hình hồi quy tuyến tính là giá trị dự đoán sự phụ thuộc tuyến tính của các giá trị đầu vào và tham số mô hình. Điều này dẫn tới khả năng tổng quát hóa của mô hình kém và không tối ưu cho dữ liệu trong thực tế. Vì vậy, mở rộng mối quan hệ phụ thuộc tuyến tính thông qua xây dựng hàm tuyến tính bằng các hàm phi tuyến sẽ giúp mô hình có tính tổng quát hơn. Các mô hình sử dụng các hàm phi tuyến với các giá trị đặc trưng đầu vào được gọi là hồi quy.

- Trong Project này, sẽ sử dụng dữ liệu ***SalesPrediction.csv*** để thực hiện dự đoán giá quảng cáo. sử dụng ***PolynomialFeatures trong sklearn.preprocessing*** để tạo các đặc trưng phi tuyến và sử dụng mô hình Linear Regression để thực hiện dự đoán.