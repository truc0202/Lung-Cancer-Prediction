# Lung-Cancer-Prediction

<a href="#"><img alt="Python" src="https://img.shields.io/badge/Python-003F5D.svg?logo=python&logoColor=white"></a>
<a href="#"><img alt="Pandas" src="https://img.shields.io/badge/Pandas-00527C.svg?logo=pandas&logoColor=white"></a>
<a href="#"><img alt="NumPy" src="https://img.shields.io/badge/Numpy-00609C.svg?logo=numpy&logoColor=white"></a>
<a href="#"><img alt="SciPy" src="https://img.shields.io/badge/SciPy-1560bd.svg?logo=scipy&logoColor=white"></a>
<a href="#"><img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-006DB2.svg?logo=python-matplotlib&logoColor=white"></a>
<a href="#"><img alt="Selenium" src="https://img.shields.io/badge/Selenium-1faecf.svg?logo=selenium&logoColor=white"></a>
<a href="#"><img alt="seaborn" src="https://img.shields.io/badge/seaborn-4E97D1.svg?logo=pandas&logoColor=white"></a>
<a href="#"><img alt="plotly" src="https://img.shields.io/badge/plotly-7BB4E3.svg?logo=plotly&logoColor=white"></a>
<a href="#"><img alt="sklearn" src="https://img.shields.io/badge/sklearn-A3CEEF.svg?logo=scikitlearn&logoColor=white"></a>
<a href="#"><img alt="NLTK" src="https://img.shields.io/badge/NLTK-C5D4EB.svg?logo=python-nltk&logoColor=white"></a>
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
![image](https://github.com/user-attachments/assets/a8d3c536-86b6-4064-b4bc-679d53a6e958)


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


## :compass:    Outline/Planning
#### 1️⃣  Data Acquisition
<details>
<summary> Gather data from Linkedin using Selenium</summary>

- Install Selenium web driver

- Create function to guide driver to automate job search

- Store data locally to a .csv file

</details>


#### 2️⃣  Data Preparation
<details>
<summary> Missing Values</summary>

- When job posting does not have enough candidates to generate insight, the **education level** and **skills** will be missing

- Missing values are manually filled by going to URL of job posting, and find another positng with the same job level, role, and company

</details>

<details>
<summary> Dummy Variables</summary>

Categorical features (e.g. `role`, `level`) are turned into dummy variables to quantify the features, so we can use them in the models.

</details>

<details>
<summary> Initial Text Cleaning</summary>

Job role names vary from companies. For example, for data scientist position, there are names like "Data Scientist II", "Data Scientist, Charging Data and Modeling", "Data Scientist - Credit Card", etc... For the purpose of analyzing the general category's relationship with the target variable, all roles are generalized to 4 categories: **Data Scientist, Data Analyst, Data Engineer, Managerial Roles**.

</details>

<details>
<summary> Parsing Text</summary>

- Convert text to all lower case for normality
	
- Remove any accented characters, non-ASCII characters
	
- Remove special characters
	
- Lemmatization
	
- Remove stopwords
	
- Store the clean text and the original text for use in future notebooks

</details>

[Preparation](preparation.ipynb)

#### :three: Data Exploration
- Address initial questions to find what are the key features that are associated with undragudate and graduate group

- Explore each feature's correlation with education distribution

- Use visualizations to better understand the relationship between features and target variable

#### :four:    Statistical Testing & Modeling	
- Conduct T-Test for categorical variable vs. numerical variable
	
- Conduct Chi^2 Test for categorical variable vs. categorical variable

- Conclude hypothesis and address the initial questions

[Exploration](exploration.ipynb)

#### :five: Modeling
- Create decision tree classifer and fit train dataset

- Find the max depth for the best performing decision tree classifer (evaluated using classification report, accuracy score)

- Create random forest classifier and fit train dataset

- Find the max depth for the best performing random forest classifier (evaluated using classification report, accuracy score)

- Create logistic regression model and fit train dataset

- Find the parameter C for the best performing logistic regression model (evaluated using classification report, accuracy score)

- Create XGBoost classifier and fit train dataset

- Pick the top 3 models among all the models and evaluate performance on validate dataset

- Pick the model with highest accuracy and evaluate on test dataset

[Modeling](modeling.ipynb)
## :repeat:   Steps to Reproduce
**NOTE:** The job postings data is not static. With that being said, the result of each run of auto-search would be different. Therefore, the insight from exploration and accuracy of models would be slightly different as well.

- [x] You will need to have a Linkedin Premium account, preferrably a premium account so you can access part of data that's used as modeling features. Store your password locally in a secret text file.
- [x] You will need to install Selenium webdrive. Please follow documentation and steps in **acquisition** notebook.
- [x] Run driver and acquire the latest job postings on your own then store it in a .csv format file.

**OR**

- [x] You can choose to use my data that I generate analysis on. Please [contact me](wang.meredith09@gmail.com) for the .csv file.

The following steps apply for both:

- [x] Clone my repo (including **imports.py**, **prepare.py**) 
- [x] Libraries used are pandas, matplotlib, seaborn, plotly, sklearn, scipy, selenium, nltk
- [x] Follow instructions in each notebook throughout the pipeline (**preparation**, **exploration**, **modeling**)and README file
- [x] Good to run workbook and read through white paper :smile_cat:

## :key:    Key Findings

<img width="952" alt="overall_distribution" src="https://user-images.githubusercontent.com/105242871/185520569-11aa7c4f-9ad1-4045-8848-54dca2f9afb3.png">

- **Less than 1/4** of data science job posting's candidate's highest education level is Bachelor degree.

- Candidate's education distribution is dependent on role (scientist, analyst, engineer, managerial roles)

- Candidate's education distribution is independent with job level (entry, associate, mid-senior)

- For entry level positions, the amount of candidates with graduate degrees is **significantly more** than those with undergrad degrees.

- Top phrases mentioned in data science job descriptions are: **Data Analytics, no. of years experience, SQL, Python, Master Degree, Business** 

- Top skills among data science candidates: **SQL, Python, Machine Learning, Data Analysis, R, C/C++, Tableau, Data Visualization**

- Final model decision tree is expected to predict with 87% accuracy on future unseen data.

<img width="805" alt="model_scores" src="https://user-images.githubusercontent.com/105242871/185667751-95813b99-9b30-4812-84c1-1a6e0f9d1e7a.png">



##  🔜    Next Steps
- For the purpose of completing a MVP, I was only able to gather 243 observations. That is one of the reason there's a class imbalance in our dataset, and why the model is failing to converge and having a higher accuracy. Therefore, gathering more data would be important.

- This project is solely focused on Data Science related job positions in the United States. We can expand the field to other areas in tech (e.g. web development, cloud administration, etc.) and compare the education distribution across fields. We can also expand countries to see if such a master-degree dominant poll is solely in the United States.

- There are extensive amount of master programs, and there is no indicator of the quality of the program itself. For further study, I would like to include parameters that distinguish different levels of degree accomplished.

## :high_brightness:    Recommendations/Further Questions
- For candidates who don't have a graduate degree, or a bachelor degree in STEM, I suggest you focus on mastering the "top skills" that we concluded in the explore section.

- What exactly is the difference between candidates who acquire the skills on their own, and those who went through a graduate program that cost $50k on average? How small is the chance for someone without a desired degree to "survive" the sea of resumes?
