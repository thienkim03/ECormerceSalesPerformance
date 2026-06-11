# Dashboard Phân Tích Hiệu Suất Bán Hàng Thương Mại Điện Tử

# Tổng quan

Dashboard được xây dựng nhằm theo dõi và đánh giá hiệu suất kinh doanh thương mại điện tử thông qua các chỉ số doanh thu, lợi nhuận, số lượng bán và đơn hàng. Dữ liệu được phân tích theo thời gian, danh mục sản phẩm và khu vực địa lý để hỗ trợ ra quyết định kinh doanh.

## Các trang Dashboard

### 1. Tổng quan

<img width="1328" height="739" alt="image" src="https://github.com/user-attachments/assets/eb563cb8-620a-4bb7-9672-6604ef4e5a0c" />

* Theo dõi các KPI chính: Doanh thu, Lợi nhuận, % Margin, Số đơn hàng và AOV.
* Phân tích xu hướng doanh thu, lợi nhuận và hiệu suất theo danh mục sản phẩm.

### 2. Phân tích theo thời gian

<img width="1319" height="720" alt="image" src="https://github.com/user-attachments/assets/c2708718-d6d0-448f-b4b5-8f955bc5fe42" />

* So sánh kết quả kinh doanh giữa các giai đoạn.
* Theo dõi biến động doanh thu, lợi nhuận và sản lượng theo thời gian.

### 3. Phân tích theo khu vực

<img width="1321" height="719" alt="image" src="https://github.com/user-attachments/assets/77853122-d1b0-4fe8-9e44-ff092e6ea353" />

* Đánh giá hiệu suất bán hàng theo thành phố và bang.
* Xác định các khu vực đóng góp doanh thu và lợi nhuận nổi bật.

## Công cụ sử dụng

**Power BI • Power Query • DAX • SQL Server**

> Phần **Insights & Recommendations** sẽ được bổ sung ở phần tiếp theo.

----

# Insights

## 1. Executive Summary

### 1.1. Doanh nghiệp chuyển từ tăng trưởng doanh thu sang tối ưu lợi nhuận

Năm 2018 ghi nhận doanh thu **272.7K**, cao hơn đáng kể so với **158.8K** của năm 2019. Tuy nhiên, lợi nhuận năm 2018 ở mức **-1.8K**, trong khi năm 2019 đạt **25.8K**.

Mặc dù quy mô kinh doanh giảm ở hầu hết các chỉ số:

* Revenue giảm 41.8%
* Quantity giảm 44.4%
* Orders giảm hơn 50%

Nhưng hiệu quả kinh doanh lại được cải thiện rõ rệt:

* Profit chuyển từ âm sang dương
* Margin tăng từ -0.7% lên 16.2%
* AOV tăng từ 833.95 lên 917.92

Điều này cho thấy doanh nghiệp đã thay đổi chiến lược kinh doanh, tập trung vào các sản phẩm và đơn hàng có khả năng sinh lời cao hơn thay vì chỉ theo đuổi tăng trưởng doanh số.

---

## 2. Profit Trend Analysis

### 2.1. Giai đoạn lợi nhuận âm trong năm 2018

Trong giai đoạn từ tháng 4 đến tháng 9 năm 2018, doanh nghiệp liên tục ghi nhận lợi nhuận âm. Đây là nguyên nhân chính khiến kết quả kinh doanh cả năm rơi vào trạng thái thua lỗ.

<img width="1348" height="346" alt="image" src="https://github.com/user-attachments/assets/5c8e8503-ac03-4339-9357-a966fcd14082" />


**Nguyên nhân chính:**

#### Furniture là danh mục tạo ra phần lớn khoản lỗ

Mặc dù đóng góp tỷ trọng doanh thu đáng kể, Furniture lại là danh mục có hiệu quả thấp nhất về mặt lợi nhuận.

<img width="1191" height="335" alt="image" src="https://github.com/user-attachments/assets/b5f59b53-dcc9-4716-bc14-fb15680781cc" />

Các sản phẩm ảnh hưởng lớn nhất:

<img width="583" height="204" alt="image" src="https://github.com/user-attachments/assets/d8399059-a305-4b64-894f-adf572bf9c0c" />

Trong đó, nhóm Tables tạo ra khoản lỗ lớn nhất và gần như triệt tiêu lợi nhuận của các danh mục còn lại.

#### Tăng trưởng doanh số không đi kèm hiệu quả tài chính

Năm 2018 ghi nhận:

* 3.6K sản phẩm được bán ra
* 277 đơn hàng
* 272.7K doanh thu

Tuy nhiên, phần lớn doanh thu đến từ các sản phẩm có biên lợi nhuận thấp hoặc âm. Điều này dẫn đến tình trạng doanh thu tăng nhưng lợi nhuận không được cải thiện tương ứng.

<img width="1330" height="337" alt="image" src="https://github.com/user-attachments/assets/2f1302a2-ac24-4e74-bb51-a14913afd19e" />


---

### 2.2. Giai đoạn lợi nhuận dương trong năm 2019

Khác với năm 2018, toàn bộ các tháng trong năm 2019 đều duy trì lợi nhuận dương.

<img width="1361" height="338" alt="image" src="https://github.com/user-attachments/assets/c5e5546c-4f57-48d8-9f44-d11db8a97763" />

Các tháng đóng góp lợi nhuận nổi bật gồm:

* January
* February
* March

<img width="1366" height="334" alt="image" src="https://github.com/user-attachments/assets/4247a33f-445d-414f-9a72-060f79c75978" />


#### Furniture được cải thiện đáng kể

<img width="1182" height="335" alt="image" src="https://github.com/user-attachments/assets/f7a5c01a-8303-4c59-bdc5-67c2e9b875e7" />

Furniture chuyển từ nhóm thua lỗ lớn nhất năm 2018 sang danh mục đóng góp lợi nhuận tích cực trong năm 2019.

Đặc biệt, Bookcases và Chairs trở thành các sản phẩm dẫn đầu về lợi nhuận trong danh mục này.

#### Electronics trở thành động lực tăng trưởng lợi nhuận

<img width="1186" height="335" alt="image" src="https://github.com/user-attachments/assets/c7e356c4-6774-4047-9415-fc4d8c8acf2f" />

Các nhóm sản phẩm đóng góp lớn nhất gồm:

* Printers
* Accessories
* Phones

Electronics là danh mục tạo ra lợi nhuận cao nhất trong năm 2019 và đóng vai trò quan trọng trong việc cải thiện kết quả kinh doanh chung.

---

## 3. Product Performance Analysis

### 3.1. Clothing là danh mục ổn định nhất

Clothing duy trì hiệu suất tích cực trong cả hai năm.

2018: 

<img width="590" height="345" alt="image" src="https://github.com/user-attachments/assets/2c1a8057-286a-4290-9267-8c6fd9043637" />

2019: 

<img width="627" height="344" alt="image" src="https://github.com/user-attachments/assets/edc8812c-2ee3-4eae-a3a5-e93a5c58614c" />



Mặc dù doanh thu giảm trong năm 2019, lợi nhuận lại tăng mạnh. Điều này cho thấy doanh nghiệp đã cải thiện được cơ cấu sản phẩm hoặc chính sách giá trong danh mục này.

Clothing là danh mục có khả năng duy trì lợi nhuận ổn định và ít biến động nhất trong toàn bộ danh mục sản phẩm.

---

### 3.2. Furniture là nguyên nhân chính gây thua lỗ năm 2018

Trong năm 2018, Furniture đóng góp đáng kể vào doanh thu nhưng lại tạo ra khoản lỗ lớn nhất.

<img width="1200" height="316" alt="image" src="https://github.com/user-attachments/assets/eb7957e0-1755-4e66-bfb0-de372aaf3a35" />

Nguyên nhân chủ yếu đến từ:

* Tables
* Chairs

Điều này cho thấy doanh nghiệp cần rà soát lại chiến lược giá bán, chi phí vận chuyển hoặc giá vốn đối với nhóm sản phẩm Furniture.

---

### 3.3. Electronics là động lực lợi nhuận năm 2019

Năm 2019, Electronics trở thành danh mục có hiệu quả kinh doanh tốt nhất.

<img width="1200" height="317" alt="image" src="https://github.com/user-attachments/assets/91f781d6-48a2-4c5a-a80f-5739bd964296" />

Danh mục này không chỉ tạo doanh thu cao mà còn duy trì biên lợi nhuận tích cực trên nhiều nhóm sản phẩm khác nhau.

---

## 4. Geographic Analysis

### 4.1. Doanh thu tập trung tại một số thành phố lớn

Trong cả hai năm, doanh thu chủ yếu tập trung ở một số thành phố dẫn đầu.

<img width="675" height="139" alt="image" src="https://github.com/user-attachments/assets/5fbde375-6749-4ddc-afdb-c6ac543ee520" />

Các thành phố như Mumbai, Indore và Pune chiếm tỷ trọng lớn trong tổng doanh thu toàn doanh nghiệp.

<img width="1364" height="348" alt="image" src="https://github.com/user-attachments/assets/7307e7cf-6b77-4892-8318-297af65f9fa6" />

---

### 4.2. Doanh thu cao không đồng nghĩa với lợi nhuận cao

Năm 2018 xuất hiện nhiều trường hợp doanh thu lớn nhưng lợi nhuận thấp hoặc âm.

[Insert bảng Top Revenue Cities vs Profit]

Ví dụ:

* Indore đạt doanh thu rất cao nhưng lợi nhuận âm.
* Mumbai có doanh thu dẫn đầu nhưng đóng góp lợi nhuận không tương xứng.

Trong khi đó, Pune lại tạo ra lợi nhuận cao dù doanh thu thấp hơn đáng kể.

Điều này cho thấy chất lượng doanh thu giữa các khu vực có sự khác biệt lớn.

---

### 4.3. Hiệu quả kinh doanh được cải thiện trên nhiều khu vực trong năm 2019

Năm 2019 ghi nhận sự cải thiện rõ rệt về lợi nhuận tại các thành phố trọng điểm.

[Insert bảng Top Profit Cities 2019]

Các thành phố đóng góp lợi nhuận cao nhất gồm:

* Indore
* Delhi
* Pune
* Kolkata

Không còn xuất hiện tình trạng doanh thu lớn nhưng lợi nhuận âm như năm 2018.

---

### 4.4. Phân bố lợi nhuận theo bang

[Insert Map Profit by State]

Lợi nhuận tập trung tại một số bang có quy mô bán hàng lớn, cho thấy doanh nghiệp đã tối ưu tốt hơn hiệu quả kinh doanh tại các thị trường trọng điểm.

Bên cạnh đó, một số bang vẫn có đóng góp doanh thu nhưng chưa tạo ra lợi nhuận tương xứng, là khu vực cần tiếp tục theo dõi trong các giai đoạn tiếp theo.

---

# Recommendations

### 1. Tập trung mở rộng các danh mục có biên lợi nhuận cao

Ưu tiên phát triển:

* Electronics
* Clothing

Đây là hai danh mục có khả năng tạo lợi nhuận ổn định và đóng góp tích cực vào kết quả kinh doanh.

### 2. Rà soát các sản phẩm từng gây thua lỗ

Đặc biệt tập trung vào:

* Tables
* Chairs

Cần đánh giá lại giá vốn, chi phí logistics và chính sách giảm giá để hạn chế nguy cơ tái diễn tình trạng thua lỗ.

### 3. Nhân rộng mô hình kinh doanh tại các khu vực hiệu quả

Các thành phố như Pune, Delhi và Indore cho thấy khả năng chuyển đổi doanh thu thành lợi nhuận tốt hơn mức trung bình.

Đây có thể là các khu vực ưu tiên trong chiến lược mở rộng kinh doanh.

### 4. Chuyển trọng tâm đánh giá từ Revenue sang Profit

Kết quả năm 2018 cho thấy doanh thu cao không đồng nghĩa với hiệu quả kinh doanh.

Do đó, Profit và Margin nên được xem là các KPI trọng tâm trong quá trình theo dõi và ra quyết định kinh doanh.


