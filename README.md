# Phân tích hành vi mua sắm thương mại điện tử

## 1. Giới thiệu

Dự án phân tích dữ liệu giao dịch thương mại điện tử nhằm tìm hiểu doanh thu, sản phẩm bán chạy, thị trường tiêu thụ và xu hướng doanh thu theo thời gian.

## 2. Dataset

- **Tên file:** `online_retail_II.xlsx`
- **Nguồn dữ liệu:** Online Retail II dataset.
- **Định dạng:** Excel (`.xlsx`).

Dữ liệu chứa thông tin hóa đơn, mã sản phẩm, mô tả sản phẩm, số lượng, ngày giao dịch, đơn giá, mã khách hàng và quốc gia.

## 3. Nội dung thực hiện

### Làm sạch dữ liệu
- Kiểm tra và loại bỏ các dòng trùng lặp.
- Kiểm tra giá trị thiếu.
- Xử lý dữ liệu giao dịch hủy.
- Loại các giao dịch có số lượng hoặc đơn giá không hợp lệ khi tính doanh thu.
- Tạo cột doanh thu bằng số lượng nhân với đơn giá.

### Phân tích khám phá dữ liệu
- Phân tích doanh thu theo tháng.
- Xác định các quốc gia có doanh thu cao.
- Phân tích sản phẩm theo doanh thu và số lượng bán.
- Trực quan hóa kết quả bằng biểu đồ.

### Phân tích hồi quy
- Xây dựng mô hình hồi quy tuyến tính để dự đoán doanh thu theo ngày.
- Chia dữ liệu theo thứ tự thời gian thành tập huấn luyện và kiểm tra.
- Đánh giá mô hình bằng MAE, RMSE và R².

## 4. Công nghệ sử dụng

- Python
- Pandas, NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Visual Studio Code

## 5. Cấu trúc dự án

```text
Khoa học dữ liệu/
├── data/
│   └── online_retail_II.xlsx
├── notebook/
│   └── analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## 6. Cách chạy dự án

1. Cài đặt các thư viện trong `requirements.txt`:

   `pip install -r requirements.txt`

2. Mở thư mục dự án bằng Visual Studio Code.

3. Mở notebook `notebook/analysis.ipynb` và chạy các cell theo thứ tự.

Lưu ý: Đường dẫn dữ liệu trong notebook cần phù hợp với cấu trúc thư mục của dự án.

## 7. Kết quả

Dự án đã thực hiện các bước làm sạch dữ liệu, phân tích khám phá và thử nghiệm mô hình hồi quy tuyến tính. Kết quả đánh giá mô hình được sử dụng để nhận xét khả năng dự đoán và những hạn chế của phương pháp.
