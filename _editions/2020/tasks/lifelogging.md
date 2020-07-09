---
# static info
layout: task
year: 2020
hide: true

# required info
title: Insight for Wellbeing
subtitle: Multimodal personal health lifelog data analysis
blurb: The quality of the air that we breathe as individuals as we go about our daily lives is important for health and wellbeing, However, measuring personal air quality remains a challenge. This task investigates the prediction of personal air quality using open data or data from lifelogs. The data includes images, tags, physiological data, and sensor readings.
---

<!-- # please respect the structure below-->

#### Task Description
Task participants create systems that derive insights from multimodal lifelog data that is important for health and wellbeing. The first dataset, namely “personal air quality data” (PAQID), includes air pollution data (PM2.5, O3, and NO2) and lifelog data (e.g., physiological data, tags, and images) collected by using sensors boxes, lifelog cameras, and smartphones along the predefined routes in a city. The second dataset, namely “global air quality data” (GAQID) includes weather and air pollution data collected over the city and provided by the government and crawled from related websites.

Participants in this task tackle two challenging subtasks:
1.	Personal Air Quality Prediction with public/open data: Task participants predict the value of personal air pollution data (PM2.5, O3, and NO2) using only weather data (wind speed, wind-direction, temperature, humidity) and air pollution data (PM2.5, O3, and NO2) from public/open data sources (e.g., stations, website).  The target of this subtask is to investigate whether we can use public/open data to predict the personal air pollution data. The personal air pollution data can be concerned as the regional air pollution data since these data a locally collected by people who carry personal equipment. In other words, the ground truth is data collected by sensor boxes carried by people.
2.	Personal Air Quality Prediction with lifelog data: participants predict the personal Air Quality Index using images captured by people (plus GAQID). The purpose of this subtask is whether we can use only lifelog data (i.e., pictures of surrounding environment, annotations and comments), weather and air pollution data from open sources to predict the personal air pollution data.

#### Motivation and Background
The association between people’s wellbeing and properties of the surrounding environment is an important area of investigation. Although these investigations have a long and rich history, they have focused on the general population. There is a surprising lack of research that investigates the impact of the environment at the scale of individual people. At personal scale, local information about air pollution (e.g. PM2.5, NO2, O3), weather (e.g. temperature, humidity), urban nature (e.g. greenness, liveliness, quietness), and personal behavior (e.g. psychophysiological data) play an important role. It is not always possible to gather plentiful amounts of such data. As the result, a key research question remains open: Can sparse or incomplete data can be used to gain insight into wellbeing? In other words, is there a hypothesis about the associations within the data so that wellbeing can be understood by using a limited amount data? Developing hypotheses about the associations within the heterogeneous data contributes towards building good multimodal models that make it possible to understand the impact of environment on wellbeing at the local and individual scale. Such models are necessary since not all cities are fully covered by standard air pollution and weather stations, and not all people experience the same reaction to the same environment situation. Moreover, images captured by the first-person view could give important cues to help understand that environmental situation in cases in which precise data from air pollution stations is lacking. 

The key research question here is “does the personal air quality can be predicted by using other data which is easy to obtain?”.

#### Target Group
This task targets (but is not limited to) researchers in the areas of multimedia information retrieval, machine learning, AI, data science, event-based processing and analysis, multimodal multimedia content analysis, lifelog data analysis, urban computing, environmental science, and atmospheric science.    

#### Data

#### Evaluation Methodology
The ground truth for the dataset of the two subtasks is collected as follows:
-	For the Personal Air Quality Prediction with public/open data subtask: some parts of personal (PM2.5, O3, and NO2) data are deleted and saved as the ground truth.
-	For the Personal Air Quality Prediction with lifelog data subtask: the set of personal AQI are hidden and saved as the ground truth  

For each subtask, the evaluation method is applied as follows:
-	For the Personal Air Quality Prediction with public/open data subtask: We use the SMAPE/RMSE/MAE for comparing each air pollution factor PM2.5, O3, and NO2 with the ground truth.
-	For the Personal Air Quality Prediction with lifelog data subtask: We use the SMAPE/RMSE/MAE for comparing predicted AQI to the ground truth.  

The formulation for computing AQI value from (PM2.5, O3, and NO2) data can be found at 
https://en.wikipedia.org/wiki/Air_quality_index (Computing the AQI section)

http://taqm.epa.gov.tw/taqm/en/b0201.aspx (is the look-up table for C_low, C_high, I_low, I_high value)

#### References and recommended reading
<!-- # Please use the ACM format for references https://www.acm.org/publications/authors/reference-formatting (but no DOI needed)-->
<!-- # The paper title should be a hyperlink leading to the paper online-->
[1] Sato, T., Dao, M.S., Kuribayashi, K., and Zettsu, K.: SEPHLA: Challenges and Opportunities within Environment – Personal Health Archives, MMM 2018. https://link.springer.com/chapter/10.1007/978-3-030-05710-7_27

[2] P. Zhao and K. Zettsu, "Decoder Transfer Learning for Predicting Personal Exposure to Air Pollution," 2019 IEEE International Conference on Big Data (Big Data), Los Angeles, CA, USA, 2019, pp. 5620-5629. https://ieeexplore.ieee.org/document/9006604

[3] N. Nguyen, M. Dao and K. Zettsu, "Complex Event Analysis for Traffic Risk Prediction based on 3D-CNN with Multi-sources Urban Sensing Data," 2019 IEEE International Conference on Big Data (Big Data), Los Angeles, CA, USA, 2019, pp. 1669-1674. https://ieeexplore.ieee.org/abstract/document/9005985

[4] P. Vo, T. Phan, M. Dao and K. Zettsu, "Association Model between Visual Feature and AQI Rank Using Lifelog Data," 2019 IEEE International Conference on Big Data (Big Data), Los Angeles, CA, USA, 2019, pp. 4197-4200. https://ieeexplore.ieee.org/document/9005636

[5] Dao, M. S., Zhao, P., Sato, T., Zettsu, K., Dang-Nguyen D. T., Gurrin, C., Nguyen, N. T.: Overview of MediaEval 2019: Insights for Wellbeing TaskMultimodal Personal Health Lifelog Data Analysis, MediaEval Benchmarking Initiative for Multimedia Evaluation (MediaEval 2019), Antipolis, France (November 2019). 

[6] Song, H., Lane, K. J., Kim, H., Kim, H., Byun, G., Le, M., Choi, Y., Park, C. R., & Lee, J. T. (2019). Association between Urban Greenness and Depressive Symptoms: Evaluation of Greenness Using Various Indicators. International journal of environmental research and public health, 16(2), 173. https://pubmed.ncbi.nlm.nih.gov/30634488/

[7] Darshan Santani, Salvador Ruiz-Correa, and Daniel Gatica-Perez. 2018. Looking South: Learning Urban Perception in Developing Cities. Trans. Soc. Comput. 1, 3, Article 13 (December 2018), 23 pages. https://dl.acm.org/doi/10.1145/3224182

[8] Anh-Vu Mai-Nguyen, Trong-Dat Phan, Anh-Khoa Vo, Van-Luon Tran, Minh-Son Dao, and Koji Zettsu. 2020. BIDAL-HCMUS@LSC2020: An Interactive Multimodal Lifelog Retrieval with Query-to-Sample Attention-based Search Engine. In Proceedings of the Third Annual Workshop on Lifelog Search Challenge (LSC ’20). Association for Computing Machinery, New York, NY, USA, 43–49. https://dl.acm.org/doi/10.1145/3379172.3391722

#### Task Organizers
Minh-Son Dao (NICT, Japan) dao@nict.go.jp
Ngoc-Thanh Nguyen (UIT, Vietnam) thanhnn.13@grad.uit.edu.vn
Peijiang Zhao (NICT, Japan)
Duc-Tien Dang-Nguyen (UiB, NOrway)
Cathal Gurrin (DCU, Ireland)

#### Task Auxiliaries
<!-- # if there are people helping with the task, but are not bearing the main responsibility for the task, they are auxiliaries. Please delete this heading if you have no auxiliaries-->
Tan-Loc Nguyen-Tai (UIT, Vietnam)
Dang-Hieu Nguyen (UIT, Vietnam)
Minh-Tam Nguyen (UIT, Vietnam)

#### Task Schedule
* 31 July: Data release <!-- # Replace XX with your date. Latest possible is 31 July-->
* 30 October: Runs due <!-- # Replace XX with your date. Latest possible is 31 October-->
* 15 November: Results returned  <!-- Fixed. Please do not change-->
* 30 November: Working notes paper  <!-- Fixed. Please do not change-->
* Early December: MediaEval 2020 Workshop <!-- Fixed. Please do not change-->

Workshop will be held online. Exact dates to be announced.
