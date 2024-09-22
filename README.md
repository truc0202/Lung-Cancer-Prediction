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
| Swallowing Difficulty          | int        | Khó khăn trong việc nuốt             |
| Clubbing of Finger Nails       | int        | Sự hiện diện của móng tay cong       |
| Frequent Cold                  | int        | Tần suất cảm lạnh          |
| Dry Cough                      | int        | Sự hiện diện của ho khan             |
| Snoring                        | int        | Tình trạng ngáy ngủ                  |
| Level                          | string           | Cấp độ chẩn đoán hoặc phân loại |


## :compass:    Outline
#### 1️⃣ Khám phá dữ liệu
- Hiểu rõ các thông tin từ các cột của dữ liệu:  Kiểm tra kiểu dữ liệu (`info()`, `dtypes`), Kích thước dữ liệu `shape`, Các biến `columns`, Lần xuất hiện `value_counts`.
- Kiểm tra và xử lý giá trị dữ liệu: Giá trị bị thiếu `isnull()`, Giá trị bị lặp `duplicated()`
- Phân phối và thống kê dữ liệu: `describe()`
#### 2️⃣  Thống kê và mô tả
##### Phân bố dữ liệu 
![image](https://github.com/user-attachments/assets/bfd014a1-f526-4b9e-ba99-1e96883305e0)
- Phân bố mức độ nghiêm trọng của bệnh nhân được phân chia thành 3 mức: Thấp (Low), Trung bình (Medium) và Cao (High).
- Tỷ lệ phân bố ở mỗi mức độ khá cân bằng: Thấp (30.30%), Trung bình (33.20%), Cao (36.50%).
- Điều này cho thấy dữ liệu thu thập được có sự phân bố đều ở các mức độ nghiêm trọng khác nhau của bệnh nhân, không bị lệch về một mức độ nào cả.
- Nói cách khác, việc thu thập dữ liệu đã được thực hiện một cách cân bằng đối với các mức độ nghiêm trọng khác nhau của bệnh nhân, đảm bảo tính đại diện của tập dữ liệu.
##### Phân chia các nhóm dữ liệu 
Dựa vào đặc điểm của những cột dữ liệu mà phân chia các cột dữ liệu vào 4 nhóm dưới: 
| **Nhân khẩu học**        | **Môi trường và lối sống** | **Tác nhân bên trong** | **Triệu chứng hô hấp**    |
|---------------------------|-----------------------------|-------------------------|----------------------------|
| Tuổi                      | Ô nhiễm không khí          | Nguy cơ di truyền       | Đau ngực                   |
| Giới tính                 | Sử dụng rượu              | Bệnh phổi mãn tính     | Ho ra máu                  |
|                           | Nguy cơ nghề nghiệp        | Béo phì                 | Mệt mỏi                    |
|                           | Chế độ ăn cân bằng         |                         | Giảm cân                   |
|                           | Hút thuốc                  |                         | Khó thở                    |
|                           | Hút thuốc thụ động         |                         | Thở khò khè                |
|                           |                             |                         | Khó nuốt                   |
|                           |                             |                         | Ngón tay dùi trống         |

<img width="600" alt="overall_distribution" src=https://github.com/user-attachments/assets/3648388c-61a6-4869-94db-01497b163eef>
<img width="600" alt="overall_distribution" src=https://github.com/user-attachments/assets/5e929fdf-d7f4-4ac7-86af-a546176d3489>
<img width="600" alt="overall_distribution" src=https://github.com/user-attachments/assets/f072a821-611d-4b9b-b79e-ed4bba87df6e>
<img width="600" alt="overall_distribution" src=https://github.com/user-attachments/assets/b95b7a49-9862-44b9-9bde-19aba45a7dce>


#### :three: Phân tích
Sau khi thống kê và chọn ra những cột dữ liệu có liên quan đến vấn đề của bài toán -> phân tích những yếu tố này với những mức độ ung thư của bệnh nhân:
![image](https://github.com/user-attachments/assets/5a8ea850-4d9f-49a5-a51a-b9c5504622f2)
Nhìn chung, các yếu tố nguy cơ như ô nhiễm không khí, nguy hiểm nghề nghiệp, bệnh phổi mãn tính, và thói quen hút thuốc có mối liên hệ mạnh với mức độ nghiêm trọng cao của bệnh ung thư.
Hầu hết những bệnh nhân thuộc mức độ cao những yếu tô trên thường có nguy cơ nghiêm trọng hơn trong bệnh ung thư phổi. Từ những điều này ta cần phải có những khuyến nghị cho mọi người để phòng và chữa bệnh.
#### :four: Áp dụng mô hình máy học
- **Bước 1:** Chọn các tính năng quan trọng
- **Bước 2:** Trực quan hóa các điểm trên các biến
- **Bước 3:** Lựa chọn các biến có điểm số cao và chuẩn bị dữ liệu
- **Bước 4:** Khởi tạo và đánh giá các mô hình Machine Learning
![image](https://github.com/user-attachments/assets/6f8880b3-49c5-4234-b5cf-4fdd59499897)
![image](https://github.com/user-attachments/assets/4d26b7a1-ee92-4f67-94d6-29857cd73afb)


## :high_brightness: Summarize & Recommendations
### Tổng kết
- Random Forest và MLP Classifier là hai mô hình nổi bật nhất với độ chính xác hoàn hảo, được khuyến nghị sử dụng cho việc phân loại dữ liệu này.
- Logistic Regression có hiệu suất thấp hơn đáng kể và không được khuyến nghị cho dữ liệu này, trừ khi cần một mô hình đơn giản và dễ giải thích.
- Decision Tree có hiệu suất cao và có thể được sử dụng khi cần giải thích dễ dàng về các quyết định của mô hình.
- KNN cũng là một mô hình mạnh, nhưng có thể không hiệu quả khi áp dụng trên các tập dữ liệu lớn hoặc khi tính toán khoảng cách giữa các điểm dữ liệu trở nên tốn kém.
  
### Đề xuất

**Đời sống:**
- Bệnh viện cần không ngừng tuyên truyền những tác nhân ảnh hưởng tới phổi như thuốc lá, rượu bia, bụi bẩn, ...
- Cung cấp hỗ trợ cai thuốc và các chương trình can thiệp giảm rượu bia.
- Khuyến khích các biện phảm giảm ô nhiễm không khí tại địa phương, như sử dụng năng lượng sạch và trồng cây.
- Nên có những chính sách ưu đãi cho khách hàng để nâng cao việc theo dõi sức khỏe định kỳ.
- Giáo dục về triệu chứng.

**Áp dụng mô hình:**
- Nên ưu tiên sử dụng Random Forest và MLP Classifier cho dự đoán ung thư phổi.
- Decision Tree có thể là lựa chọn tốt trong các tình huống cần giải thích rõ ràng.
- Logistic Regression và KNN có thể được xem xét trong các trường hợp cụ thể, nhưng cần hiểu rõ về hạn chế của chúng.
