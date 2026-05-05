 **Patient Flow and Hospital Performance Analysis Using Business Intelligence and Data Analytics**

🏥 Al-Haramain Hospital BI Dashboard & Analytics
Authors

Malak Hababih,Maya salahi

Supervised by:
Dr.husam barham

University:
University of Petra

Course:
Graduation Project

Semester:
Second Semester, 2025/2026

Date:1/6/2026
## **Table of Content**
1. Abstract  
2. Acknowledgment  
3. Project Description and Objectives  
4. Data Research and Acquiring Effort  
5. Data Description and Understanding  
6. Data Cleaning and Transformation  
7. Data Visualization and Insights  
8. Dashboard Design & Business Insights  
9. Tools and Technologies  
10. Project Deployment  
11. Results  
12. References
## **Abstract**
This project focuses on analyzing hospital data from Al-Haramain Hospital to understand patient behavior and improve healthcare operations by leveraging data analysis and business intelligence techniques. The main objective is to transform large volumes of raw hospital data into meaningful insights that support decision-making. By identifying patient distribution across departments, analyzing patient flow, detecting peak times in the emergency department, and evaluating length of stay, the project aims to highlight key operational challenges and improve overall hospital performance. Additionally, basic forecasting techniques are used to provide a general view of future patient demand.

The implementation process involved collecting and integrating data from multiple hospital records, followed by data cleaning and preprocessing to ensure consistency and accuracy. Missing values were handled, date formats were standardized, and relevant features were prepared for analysis. Various analytical techniques were applied using Python to explore patient trends, department workloads, and temporal patterns. Patient flow between departments was analyzed to understand movement patterns within the hospital. The processed data was then exported and visualized using Tableau, where interactive dashboards were developed to present insights through charts, filters, and comparative views.

The results reveal clear patterns in patient distribution and hospital operations. The Emergency Department showed the highest number of patient visits, indicating significant pressure compared to other departments. Analysis also identified peak times during specific hours and days, as well as variations in length of stay across departments. Patient flow analysis highlighted common transition paths between departments, reflecting the internal workflow of the hospital. Forecasting results provided a general indication of future patient demand trends. The interactive dashboards allow users to explore these insights dynamically, supporting better resource allocation, reducing waiting times, and enhancing the overall quality of healthcare services through data-driven decision-making.
## **Acknowledgment**

I would like to express my sincere gratitude to my academic supervisors and instructors for their continuous guidance, valuable feedback, and support throughout the development of this project. Their direction played a key role in shaping both the analytical and practical aspects of this work. I would also like to acknowledge the use of tools and technologies such as Python, Google Colab, and Tableau, which greatly facilitated the data analysis and visualization processes. Finally, I extend my appreciation to everyone who supported me during this project, whether through advice, resources, or encouragement, contributing to the successful completion of this graduation project.
## **Business Intelligence Project Description and Objectives**
 This project aims to analyze hospital operations and patient behavior using healthcare data from Al-Haramain Hospital. The healthcare sector is one of the most critical industries, as it directly affects human well-being and quality of life. With the increasing adoption of data-driven systems, hospitals generate large volumes of data that can be leveraged to improve efficiency and decision-making.

Despite the availability of data, hospitals often face challenges such as long waiting times, inefficient patient flow, and suboptimal resource allocation. These issues arise mainly due to the lack of effective data analysis and utilization.

To address this problem, this project applies Business Intelligence techniques to transform raw hospital data into meaningful and actionable insights. By analyzing patient distribution, department activity, patient flow, and length of stay, the project helps identify operational inefficiencies and performance gaps.

The project follows a complete BI pipeline, starting from data collection and preprocessing to ensure data quality, and ending with the development of an interactive dashboard using Tableau. This dashboard enables stakeholders to monitor performance, detect trends, and make informed decisions.

Additionally, the project analyzes temporal patterns in patient visits to identify peak hours, days, and seasonal trends. It also examines patient movement across departments to detect bottlenecks and evaluates the length of stay to highlight departments with extended durations.

Project Objectives
Analyze patient distribution and hospital workload
Identify peak hours, days, and high-demand periods
Understand patient flow between departments and detect bottlenecks
Evaluate length of stay across departments
Improve resource allocation and operational efficiency
Support data-driven decision-making through interactive dashboards
## **Data Research and Acquiring Effort**

operational workflows within Al-Haramain Hospital. Since the main objective of the project is to analyze patient behavior and evaluate hospital performance, the dataset needed to capture real interactions such as patient admissions, department transitions, and duration of stay.

During the data research phase, multiple potential data sources were explored, including publicly available healthcare datasets and online repositories. However, many of these datasets were either pre-processed, limited in size, outdated, or lacked critical attributes required for this analysis. In several cases, these datasets did not include important fields such as timestamps, patient movement between departments, or complete admission and discharge records. Additionally, relying on multiple datasets would introduce integration challenges, increase preprocessing complexity, and potentially lead to inconsistencies in the analysis.

To overcome these limitations and ensure data reliability and realism, a structured dataset representing actual hospital operations was utilized. This dataset was specifically designed to reflect real patient interactions within the hospital environment. It includes key attributes such as patient ID, department name, visit date, admission and discharge timestamps, and transitions between departments.

The dataset contains approximately [83,000] patient records, collected over a defined time period, enabling both behavioral and operational analysis. These attributes were carefully selected to support multiple analytical perspectives, including patient distribution, department workload, patient flow between departments, and temporal trends.

By working with structured hospital data, full control was maintained over the attributes used in the analysis. This ensured that the dataset was directly aligned with the project objectives, rather than adapting the analysis to fit the limitations of external datasets.

A significant effort was dedicated to data cleaning and preprocessing. This process involved handling missing values, correcting inconsistencies, removing duplicate records, and standardizing date and time formats. Ensuring proper datetime formatting was particularly important for calculating accurate metrics such as length of stay and for enabling time-based analysis.

The data was processed and analyzed using Python in Google Colab. Various preprocessing techniques and feature engineering steps were applied, including extracting time components such as year, month, and day from admission dates. Additional calculated fields, such as length of stay, were created to support deeper analysis.

After preprocessing, the cleaned dataset was exported and integrated into Tableau for visualization and dashboard development. This allowed the creation of interactive dashboards that present key insights in a clear and structured manner.

Special attention was given to analyzing patient movement between departments (Patient Flow), as it provides valuable insights into hospital efficiency, resource utilization, and potential operational bottlenecks. Additionally, the dataset supported analysis of department workload differences and patient stay durations.

Overall, this structured approach to data acquisition and preparation ensured that the dataset is accurate, relevant, and suitable for Business Intelligence analysis. The resulting insights contribute to a better understanding of hospital operations and support data-driven decision-making.
Dataset:
Figure 1: Raw dataset showing hospital patient records.
<img width="1606" height="710" alt="Screenshot 2026-05-05 201242" src="https://github.com/user-attachments/assets/e06c2457-9dce-456f-9539-a1b304ae4f7f" />
<img width="723" height="710" alt="Screenshot 2026-05-05 202412" src="https://github.com/user-attachments/assets/10f44db1-7026-4bd4-be56-f977a965afd8" />
<img width="762" height="725" alt="Screenshot 2026-05-05 202342" src="https://github.com/user-attachments/assets/11198788-3d36-4ac6-9065-1bebab7f378c" />
<img width="610" height="712" alt="Screenshot 2026-05-05 202320" src="https://github.com/user-attachments/assets/7fb3c718-46c5-46a7-ae22-c7fe148d942f" />
<img width="1694" height="709" alt="Screenshot 2026-05-05 202221" src="https://github.com/user-attachments/assets/425ddb45-6ef8-48ff-b01f-861a5601ccff" />

Data cleaning
The following step shows data cleaning operations performed to handle missing values and inconsistencies.
<img width="403" height="689" alt="Screenshot 2026-05-05 202829" src="https://github.com/user-attachments/assets/5dc212d6-0898-4a84-bb26-803ae2414219" />
datetime:
<img width="826" height="124" alt="Screenshot 2026-05-05 202958" src="https://github.com/user-attachments/assets/a75dc571-ad51-4a40-8109-6675dc1df6ab" />
The following visualization was created using Tableau to analyze patient distribution across hospital departments and identify workload differences between departments.<img width="1233" height="843" alt="Screenshot 2026-05-05 204559" src="https://github.com/user-attachments/assets/5d0bdd70-af5a-4481-bcf8-3474e3dffd7e" />

## **Data Description and Understanding**
The dataset used in this project represents operational and patient-related data from Al-Haramain Hospital. It captures real hospital activities such as patient admissions, visits to different departments, transfers between departments, and discharge information.

The data is structured in a tabular format where each row represents a single patient visit or interaction within the hospital system. This structure allows tracking the full patient journey across different departments.

The dataset includes several key attributes such as Patient ID, Department Name, Admission Time, Discharge Time, Gender, Reason for Visit, and other operational fields. These attributes enable a comprehensive understanding of patient behavior and hospital operations.

From initial exploration, the dataset contains multiple departments such as Emergency, Laboratory, Pharmacy, and Radiology. This allows analysis of patient distribution across departments and understanding of internal hospital workflows.

The data is time-based, which makes it suitable for temporal analysis such as identifying peak hours, daily trends, and length of stay calculations. Proper datetime formatting plays an important role in ensuring accurate analysis.

Overall, the dataset provides a rich and structured representation of hospital operations, making it suitable for Business Intelligence analysis and supporting insights into patient flow, workload distribution, and operational efficiency.
## **Data Primary Cleaning and Transformation**
The raw dataset underwent a thorough cleaning and preprocessing phase to ensure data quality, consistency, and reliability for analysis. This step was essential to prepare the data for accurate Business Intelligence insights.

During the cleaning process, missing values were identified and handled appropriately depending on the context of each attribute. Duplicate records were also checked and removed to avoid redundancy and ensure data accuracy.
<img width="337" height="45" alt="Screenshot 2026-05-05 211542" src="https://github.com/user-attachments/assets/4e451373-643c-4164-a49f-be041bb01a38" />
<img width="821" height="131" alt="Screenshot 2026-05-05 211852" src="https://github.com/user-attachments/assets/b5a64c9a-1181-48e9-9781-39b7db4360f4" />

A significant part of the preprocessing involved handling datetime fields. Admission and discharge timestamps were converted into a consistent datetime format, enabling accurate calculation of time-based metrics such as length of stay and visit duration.
<img width="826" height="124" alt="Screenshot 2026-05-05 202958" src="https://github.com/user-attachments/assets/b1535f5d-690e-4ec2-81b8-67a3d17adc0b" />

Feature engineering was also applied to enhance the dataset. New attributes such as year, month, day, and time components were extracted from the original datetime fields to support temporal analysis and trend identification.
<img width="612" height="363" alt="Screenshot 2026-05-05 212406" src="https://github.com/user-attachments/assets/85bc095a-acb0-4465-b008-fccaa4a00602" />

Finally, the cleaned dataset was structured and exported for further analysis and visualization in Tableau. This transformation process ensured that the data was fully prepared, consistent, and suitable for generating reliable insights in the next stages of the project.
## **Data Visualization and Insights**
The following visualization illustrates the **patient flow between different hospital departments**. It helps in understanding how patients move within the hospital system and identifies common transition paths and operational bottlenecks.
<img width="1452" height="778" alt="Screenshot 2026-05-05 212922" src="https://github.com/user-attachments/assets/150a1bcc-ccf4-48d1-aa38-c0ca6aa32cf4" />
The analysis of patient flow shows that most patients start their journey in the Emergency Department before moving to the Laboratory or Radiology departments for further diagnosis.
It is also observed that there are frequent transitions between Laboratory and Pharmacy, indicating a strong dependency between diagnostic and treatment stages.
These patterns highlight key operational workflows within the hospital and help identify potential bottlenecks that may affect patient waiting times and resource utilization.

The following visualization shows the **distribution of patient visits across different hospital departments**. This chart helps in understanding the workload and demand levels for each department within Al-Haramain Hospital.
<img width="1233" height="843" alt="Screenshot 2026-05-05 204559" src="https://github.com/user-attachments/assets/36fbedaa-3b3f-44b6-881b-5741c2254f4f" />
The results indicate that the Emergency Department has the highest number of patient visits compared to other departments, showing that it is the most frequently used service point in the hospital
The Laboratory and Pharmacy departments also show a relatively high number of visits, which reflects their important role in patient diagnosis and treatment processes.
Some departments like Radiology have fewer patients because they are used less often or only in special cases.
These findings help in understanding department workload distribution and support better resource allocation and staffing decisions.

The following visualization presents the **daily trend of patient visits over time**. It helps in understanding how patient demand changes on a day-to-day basis within Al-Haramain Hospital.
<img width="1447" height="753" alt="Screenshot 2026-05-05 214639" src="https://github.com/user-attachments/assets/8e595377-8c73-4c5a-b2b6-a8ae211abc76" />
The daily trend shows that patient visits are lower on Fridays compared to other days, indicating it is the least busy day in the hospital.
In contrast, Mondays show the highest number of patient visits, reflecting a peak in hospital demand at the beginning of the week.
This pattern suggests that patient flow is influenced by weekly routines, which should be considered when planning 

The following visualization presents the **time trend of patient visits across different months and years**. It helps in identifying long-term patterns in hospital demand over time.
<img width="1449" height="765" alt="Screenshot 2026-05-05 220419" src="https://github.com/user-attachments/assets/c1222f10-8992-45c7-92be-a43eaca75d5a" />
The analysis shows that patient visits increased significantly over time, reaching a peak around 2023–2024, followed by a noticeable decline afterward.

Monthly patterns also show fluctuations in patient volumes, where some months record higher values compared to others.
These variations reflect changes in hospital activity over time; however, the exact causes cannot be determined from the dataset alone.

The following visualization shows the **frequency of patient visits**in the dataset.
<img width="1452" height="761" alt="Screenshot 2026-05-05 221434" src="https://github.com/user-attachments/assets/300447f8-e70b-4043-8b8a-37ae70d7166e" />
Most patients have low visit frequency, while a small number of patients account for repeated visits across the hospital system.
This pattern may be explained by the fact that many cases treated in the hospital are one-time or short-term treatments, while only a smaller group of patients require follow-up visits or continuous care for ongoing health conditions.

The following visualization shows the distribution of **patient length of stay across hospital departments**.
<img width="1435" height="759" alt="Screenshot 2026-05-05 221915" src="https://github.com/user-attachments/assets/0bcf79ad-9a67-4cfb-adf8-6f766ede94a7" />
The results show that the Emergency and Treatment departments have the longest patient stays, while the Pharmacy department shows no length of stay since it only involves dispensing medication without patient admission.

The following visualization shows the **peak admission hours analysis**, illustrating the distribution of patient admissions across different hours of the day.
<img width="1444" height="760" alt="Screenshot 2026-05-05 222627" src="https://github.com/user-attachments/assets/48b3f1af-55d4-4137-a93c-3413ff9c039d" />
The analysis shows that the highest number of patient admissions occurs around 8–9 PM, indicating peak hospital activity during the evening hours. In contrast, the lowest admission rate is observed around 5 AM, when hospital demand is at its minimum.
This pattern suggests that most patients tend to seek medical care during evening hours after daily activities, while early morning hours experience significantly lower demand.
Based on these findings, it is recommended to allocate more medical staff and resources during peak evening hours to improve service efficiency and reduce patient waiting time, while maintaining minimal staffing during early morning hours.
## **Dashboard Design & Business Insights**

## **Advanced Analytics and AI Modeling**

## **Tools Research and Selection Effort**

## **Project Deployment Effort – Use Case**

## **Results**

## **References**


