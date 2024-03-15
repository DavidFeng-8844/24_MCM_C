# 2024 MCM Math Modeling Task C 
Utilize a range of machine-learning algorithms, including
LGBM, XGBoost, Support Vector Machines, Perceptron Networks, and Logistic Regression
to analyze the momentum changes in the Tennis match
## Problem Analysis
The problem analysis consists of four studies:

1. Identifying factors influencing tennis players' scoring abilities, employing logistic regression and machine learning techniques.
2. Investigating the significance of "momentum" in matches through predictive modeling and correlation analysis.
3. Adapting models to predict performance fluctuations across games, utilizing logistic regression and support vector machines.
4. Validating model performance across matches and proposing future research directions, demonstrating the system's applicability and generalizability.
## Model Construction 
### Data Preprocessing
In the initial phase of data preprocessing, the dataset is imported from a .csv file, and
the Pandas library is employed to structure the data into a DataFrame. After
this, the dropna function is applied to eliminate records with missing values. Following
the initial data preparation, the script undertakes a comprehensive feature engineering
process, introducing novel features pertinent to the distinct characteristics of tennis
matches.

In the subsequent phase, the dataset is readied for modelling through a meticulous
iteration over each data point. This involves the extraction of features and the assignment of labels contingent upon the outcome of each point, specifically focusing on
point victories. To enhance the robustness and suitability of the data for subsequent
machine learning applications, the features undergo scaling. The MinMaxScaler from
the scikit-learn library is employed for this purpose, ensuring that all variables are
standardized within the [0, 1] range. This standardization is imperative to mitigate the
undue influence of certain features during the modeling process, arising from variations
in scale.

The finalization of the preprocessing sequence involves the preservation of the pro-
cessed and standardized dataset in an Excel file. These methodical steps collectively
address challenges associated with missing values, outliers, and standardization, culmi-
nating in the generation of a refined dataset poised for efficacious utilization in machine
learning endeavors

## Model Assumption
- The server holds an advantage over the receiver, implying that initiating the serve increases the likelihood of gaining an upper hand.
- Players are influenced by match "momentum," where past success or failure affects future performance, indicating its crucial role in game outcomes.
- A player's technical skill directly impacts scoring performance, emphasizing the significance of individual abilities in point acquisition.
- Fatigue affects players during matches, diminishing performance as the game progresses due to declining energy levels.
- The psychological state of players significantly influences matches, including their ability to handle mistakes and critical moments, highlighting the importance of mental toughness and readiness for success in competition.

## Symbol Description 
![image](https://github.com/DavidFeng-8844/24_MCM_C/assets/110443929/b0ce170c-81e5-4f28-b058-aa4d085f965c)

## Statistical Logistic Regression Analysis Based on Indicator System
This study utilizes a comprehensive indicator system to evaluate the real-time scoring of players in sports matches. The system enables scoring calculations for each point in every set of every match, accompanied by assessments of current performance indicators. Validation of these indicators' significance in point scoring is conducted through statistical regression analysis, employing a binary logistic regression model in SPSS software.

![image](https://github.com/DavidFeng-8844/24_MCM_C/assets/110443929/57b6aca8-9972-44f4-b397-d08c959d3362)

The logistic regression analysis in SPSS yields an overall accuracy of 65.5%. The model demonstrates a classification accuracy of 34.4% for instances where players genuinely did not score, and a significantly higher accuracy of 85.2% for instances where players did score, indicating a preference for classifying samples where players actually scored (label 1).

However, it's essential to recognize that this logistic regression analysis serves a prospective examination purpose. Its aim is to determine whether the constructed indicators significantly influence players' actual scoring situations. The results of the logistic regression analysis are presented in a subsequent table.

![image](https://github.com/DavidFeng-8844/24_MCM_C/assets/110443929/2f00f20d-10ec-4b96-a71d-505b149d468f)

## Other Methods
![image](https://github.com/DavidFeng-8844/24_MCM_C/assets/110443929/7d6acd18-6352-4cd6-a8a8-dca576ef913c)

![image](https://github.com/DavidFeng-8844/24_MCM_C/assets/110443929/c72904b7-616e-441a-bd5f-3ca279a06bf3)

![image](https://github.com/DavidFeng-8844/24_MCM_C/assets/110443929/56d8498b-6e8c-4ca5-b7f7-92774c99ee5c)
