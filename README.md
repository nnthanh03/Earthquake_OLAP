# Phân tích dữ liệu kho động đất với OLAP (SSIS, SSRS, Power BI)

## Giới thiệu
Dự án này nhằm phân tích dữ liệu động đất sử dụng các công cụ OLAP như SSIS, SSRS và Power BI. Chúng tôi đã xây dựng kho dữ liệu, thực hiện truy vấn, tạo báo cáo và khai thác dữ liệu bằng Data Mining.

## Mục lục
1. [Tổng quan đề tài](#tong-quan-de-tai)
2. [Xây dựng kho dữ liệu](#xay-dung-kho-du-lieu)
3. [Quá trình ETL với SSIS](#etl-ssis)
4. [Phân tích dữ liệu với SSAS](#phan-tich-du-lieu-ssas)
5. [Báo cáo với SSRS và Power BI](#bao-cao-ssrs-powerbi)
6. [Khai thác dữ liệu với Data Mining](#data-mining)
7. [Các nguồn tài liệu tham khảo](#tai-lieu-tham-khao)

---

## 1. Tổng quan đề tài <a name="tong-quan-de-tai"></a>
### 1.1 Lý do chọn đề tài
- Hiểu rõ hơn về các trận động đất trên toàn thế giới.
- Áp dụng các kỹ thuật OLAP để tối ưu phân tích dữ liệu lớn.

### 1.2 Mô tả dữ liệu
- Dữ liệu gốc: Bao gồm thông tin về thời gian, vị trí, cường độ và số trạm quan sát.
- Kho dữ liệu đã xử lý: Được chuẩn hóa và đã xây dựng theo lược đồ hình sao (Star Schema).

## 2. Xây dựng kho dữ liệu <a name="xay-dung-kho-du-lieu"></a>
- Thiết kế lược đồ hình sao.
- Xây dựng các bảng Dim_Location, Dim_MagType, Dim_Network, Dim_Time và Fact_Earthquake.
- Tạo các ràng buộc khóa ngoại.

## 3. Quá trình ETL với SSIS <a name="etl-ssis"></a>
- Tạo project SSIS và thiết lập kết nối.
- Import dữ liệu và xử lý dữ liệu.
- Xây dựng các gói (Package) để load dữ liệu vào kho.

## 4. Phân tích dữ liệu với SSAS <a name="phan-tich-du-lieu-ssas"></a>
- Tạo project SSAS và điều chỉnh Dimensions.
- Thực hiện các truy vấn MDX để phân tích dữ liệu.
- Trả lời các truy vấn như: tổng số trận động đất theo khu vực, theo thời gian, top khu vực có số trận động đất nhiều nhất...

## 5. Báo cáo với SSRS và Power BI <a name="bao-cao-ssrs-powerbi"></a>
- Tạo báo cáo với SSRS.
- Trực quan hóa dữ liệu bằng Power BI.

## 6. Khai thác dữ liệu với Data Mining <a name="data-mining"></a>
- Sử dụng các thuật toán:
  - Decision Tree
  - Clustering
  - Naïve Bayes
- Đánh giá độ chính xác bằng Mining Accuracy Chart.

## 7. Các nguồn tài liệu tham khảo <a name="tai-lieu-tham-khao"></a>
- [USGS Earthquake Data](https://earthquake.usgs.gov/)
- Tài liệu chính thức từ Microsoft về SSIS, SSRS, SSAS.

## Cách sử dụng
1. Clone repository: `git clone https://github.com/nnthanh03/Earthquake_OLAP.git`
2. Mở các project SSIS, SSAS trong Visual Studio.
3. Chạy các package SSIS để load dữ liệu.
4. Triển khai SSAS và SSRS.
5. Xem báo cáo trên Power BI.


