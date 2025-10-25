# Phân loại ảnh Fashion MNIST bằng TensorFlow/Keras

## Giới thiệu 

Đây là project thực hành xây dựng một model ANN đơn giản bằng thư viện TensorFlow và Keras để phân loại các hình ảnh trong bộ dữ liệu **Fashion MNIST**.

Mục tiêu là xây dựng và huấn luyện một mô hình có khả năng nhận diện các loại trang phục khác nhau (áo thun, quần, giày, v.v.) từ ảnh grayscale kích thước 28x28 pixel.

## Nội dung chính 

File `tf_fashion_mnist.ipynb` bao gồm các bước sau:

1.  **Tải và khám phá dữ liệu:** Tải bộ dữ liệu Fashion MNIST từ `keras.datasets` và trực quan hóa một vài hình ảnh mẫu.
2.  **Tiền xử lý dữ liệu:**
    * Chuẩn hóa giá trị pixel của ảnh về khoảng \[0, 1].
    * Thêm chiều channel dimension.
    * Chuyển đổi label sang dạng one-hot encoding.
3.  **Xây dựng mô hình:** Định nghĩa kiến trúc mạng ANN đơn giản sử dụng `keras.Sequential` với các lớp `Flatten` và `Dense`.
4.  **Compile mô hình:** Thiết lập optimizer, loss function và metrics.
5.  **Huấn luyện mô hình:** Sử dụng `model.fit()` để huấn luyện mô hình trên tập dữ liệu huấn luyện (`x_train`, `y_train_label`) và đánh giá trên tập kiểm thử (`validation_split`).
6.  **Đánh giá mô hình:**
    * Vẽ biểu đồ thể hiện sự thay đổi của `loss` và `accuracy` trên tập huấn luyện và kiểm thử qua các epoch.
    * Sử dụng `model.evaluate()` để tính toán `loss` và `accuracy` cuối cùng trên tập dữ liệu test (`x_test`, `y_test_label`).
7.  **Dự đoán:** Sử dụng `model.predict()` để dự đoán nhãn cho một vài ảnh mẫu từ tập test và trực quan hóa kết quả dự đoán cùng labels thật.

## Công nghệ sử dụng 

* **Python**
* **TensorFlow**
* **Keras**
* **NumPy**
* **Matplotlib**

## Nguồn tham khảo 

Code trong project này được thực hiện dựa trên hướng dẫn từ video YouTube sau:

* **Tên Kênh:** CodeXplore
* **Link:** [https://www.youtube.com/watch?v=a4-hBti_sLo](https://www.youtube.com/watch?v=-E-s6QYy-Mc)
---
