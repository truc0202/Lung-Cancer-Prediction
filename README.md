# Lung-Cancer-Prediction

<a href="#"><img alt="Python" src="https://img.shields.io/badge/Python-003F5D.svg?logo=python&logoColor=white"></a>
<a href="#"><img alt="Pandas" src="https://img.shields.io/badge/Pandas-00527C.svg?logo=pandas&logoColor=white"></a>
<a href="#"><img alt="NumPy" src="https://img.shields.io/badge/Numpy-00609C.svg?logo=numpy&logoColor=white"></a>
<a href="#"><img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-006DB2.svg?logo=python-matplotlib&logoColor=white"></a>
<a href="#"><img alt="seaborn" src="https://img.shields.io/badge/seaborn-4E97D1.svg?logo=pandas&logoColor=white"></a>
<a href="#"><img alt="sklearn" src="https://img.shields.io/badge/sklearn-A3CEEF.svg?logo=scikitlearn&logoColor=white"></a>
## :globe_with_meridians:   Project Description
Lĩnh vực: Y tế.
Bối cảnh vấn đề:
+ Ung thư phổi là một mối đe dọa sức khỏe toàn cầu, chiếm vị trí thứ hai trong số các loại ung thư phổ biến ở Hoa Kỳ và là loại ung thư gây tử vong hàng đầu trên toàn thế giới. 
+ Điều đáng lo ngại là ung thư phổi thường được phát hiện muộn, khi bệnh đã tiến triển và khó điều trị. 
+ Nhiều bệnh nhân không có triệu chứng trong những giai đoạn đầu, khiến việc chẩn đoán sớm trở nên khó khăn. 

## :star2:  Project Goals
Mục tiêu của dự án:
+ Mặc dù không có nguyên nhân duy nhất gây ra ung thư phổi, nhưng bằng cách phân tích các bộ dữ liệu liên quan, chúng ta có thể xác định một số yếu tố nguy cơ tiềm ẩn, từ đó hỗ trợ việc dự đoán, sàng lọc và điều trị bệnh hiệu quả hơn.
+ Dự án này hướng đến việc ứng dụng kỹ thuật máy học để phân tích dữ liệu liên quan đến bệnh nhân ung thư phổi, nhằm mục tiêu:

	▪ Xây dựng mô hình phân loại: Phát triển một mô hình máy học có khả năng dự đoán bệnh nhân ở giai đoạn ung thư nào dựa trên các yếu tố v.v.

	▪ Hỗ trợ và cải thiện điều trị: Phân tích dữ liệu để xác định các yếu tố ảnh hưởng  và sử dụng mô hình dự đoán để phát hiện sớm mức độ những bệnh nhân để hỗ trợ việc sàng lọc và hỗ trợ điều trị hiệu quả hơn.
## :memo:   Initial Questions
<img width="700" alt="overall_distribution" src=https://github.com/user-attachments/assets/a8d3c536-86b6-4064-b4bc-679d53a6e958>


## :open_file_folder:   Data Dictionary

| **Biến**                       | **Loại giá trị** | **Ý nghĩa**                                                 |
|--------------------------------|------------------|------------------------------------------------------------|
| Patient Id                     | string            | Mã định danh duy nhất cho mỗi bệnh nhân                    |
| Age                            | int        | Tuổi của bệnh nhân tính bằng năm                           |
| Gender                         | int        | Giới tính của bệnh nhân         |
| Air Pollution                  | int        | Mức độ tiếp xúc với ô nhiễm không khí |
| Alcohol use                    | int        | Tần suất tiêu thụ rượu                |
| Dust Allergy                   | int        | Sự hiện diện của dị ứng bụi            |
| OccuPational Hazards           | int        | Tiếp xúc với nguy cơ nghề nghiệp      |
| Genetic Risk                   | int        | Xu hướng di truyền đến bệnh phổi      |
| chronic Lung Disease           | int        | Tiền sử bệnh phổi mãn tính            |
| Balanced Diet                  | int        | Chất lượng chế độ ăn            |
| Obesity                        | int        | Sự hiện diện của béo phì              |
| Smoking                        | int        | Tình trạng hút thuốc  |
| Passive Smoker                 | int        | Tiếp xúc với khói thuốc               |
| Chest Pain                     | int        | Sự hiện diện của đau ngực            |
| Coughing of Blood              | int        | Sự cố ho ra máu                       |
| Fatigue                        | int        | Cảm giác mệt mỏi                      |
| Weight Loss                    | int        | Giảm cân không mong muốn              |
| Shortness of Breath            | int        | Các đợt khó thở                       |
| Wheezing                       | int        | Sự hiện diện của khò khè             |
| Swallowing Difficulty          | int      500" alt="overall_distribution" src=https://github.com/user-attachments/assets/b95b7a49-9862-44b9-9bde-19aba45a7dce>

#### :three: Phân tích
![image](https://github.com/user-attachments/assets/101bbab2-dbd1-45b3-b86e-f68bab05fe52)

#### :four: Áp dụng mô hình máy học
- **Bước 1:** Chọn các tính năng quan trọng
- **Bước 2:** Trực quan hóa các điểm trên các biến
- **Bước 3:** Lựa chọn các biến có điểm số cao và chuẩn bị dữ liệu
- **Bước 4:** Khởi tạo và đánh giá các mô hình Machine Learning
![image](https://github.com/user-attachments/assets/6f8880b3-49c5-4234-b5cf-4fdd59499897)
![image](https://github.com/user-attachments/assets/4d26b7a1-ee92-4f67-94d6-29857cd73afb)


## :high_brightness: Summarize & Recommendations
**Tổng kết** 
- Random Forest và MLP Classifier là hai mô hình nổi bật nhất với độ chính xác hoàn hảo, được khuyến nghị sử dụng cho việc phân loại dữ liệu này.
- Logistic Regression có hiệu suất thấp hơn đáng kể và không được khuyến nghị cho dữ liệu này, trừ khi cần một mô hình đơn giản và dễ giải thích.
- Decision Tree có hiệu suất cao và có thể được sử dụng khi cần giải thích dễ dàng về các quyết định của mô hình.
- KNN cũng là một mô hình mạnh, nhưng có thể không hiệu quả khi áp dụng trên các tập dữ liệu lớn hoặc khi tính toán khoảng cách giữa các điểm dữ liệu trở nên tốn kém.
**Đề xuất**
- 
