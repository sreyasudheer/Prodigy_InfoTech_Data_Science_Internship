# Prodigy_InfoTech_Data_Science_Internship
This repository contains my data science internship tasks at Prodigy InfoTech.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------


# Global Population Analysis (PRODIGY_DS_01)

## Overview
This repository contains the Exploratory Data Analysis (EDA) of global population trends. The project aims to visualize and summarize demographic distribution and identify the most populous nations using historical data spanning from 2001 to 2022.

## 🎯 Objective
The primary objective of this analysis is to:
* Understand global population distribution patterns.
* Identify the top-ranking countries by population size in 2022.
* Observe population growth trends over a 20-year period.

## 📊 Data Description
* **Dataset:** `worldpopulationdata.csv`
* **Dataset Details:** The file includes 1,085 entries with demographic information. 
* **Key Variables:** Country Name, Country Code, and annual population counts from 2001 to 2022.
* **Preprocessing:** Data was filtered to isolate the 'Total Population' series (SP.POP.TOTL) to ensure consistency and accuracy in the reporting.

## 🛠 Tools Used
* **Languages:** Python
* **Libraries:** 
    * `pandas`: Used for data manipulation and cleaning.
    * `matplotlib` & `seaborn`: Used for generating visualizations.
* **Environment:** Jupyter Notebooks

## ⚙️ Methodology
1. **Data Cleaning:** The dataset was cleaned to ensure numerical integrity for annual population columns.
2. **Exploratory Data Analysis (EDA):** Calculated descriptive statistics including mean, median, and standard deviation to understand the global data spread.
3. **Visualization:** Generated horizontal bar charts to provide a comparative analysis of the top 10 most populous countries in 2022.

## 📈 Results & Findings
* **Population Distribution:** The mean population across recorded entries in 2022 was approximately 14.6 million, though with a high standard deviation, indicating a massive disparity between smaller territories and major nations.
* **Key Findings:** India and China represent the highest population brackets globally, significantly outpacing all other nations in the dataset.
* **Insights:** The analysis confirms that the population is heavily concentrated in a few key nations, which influences global economic and social trends.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------


# Titanic Passenger Exploratory Data Analysis

## 🎯 Project Objective
The objective of this project is to perform a comprehensive Exploratory Data Analysis (EDA) on the Titanic passenger dataset. The goal is to understand the underlying passenger demographics, identify data quality issues, and uncover insights that inform future predictive modeling and machine learning applications.

## 📊 Data Description
The dataset contains **418 records** covering various attributes of Titanic passengers[cite: 7]. Key features include:
*   **Passenger Identity**: Unique IDs, names, and ticket numbers[cite: 7].
*   **Demographics**: Age and Sex[cite: 7].
*   **Socio-Economic Indicators**: `Pclass` (Ticket class) and `Fare`[cite: 7].
*   **Logistics & Family**: `SibSp` (siblings/spouses), `Parch` (parents/children), `Cabin`, and `Embarked` (port of embarkation)[cite: 7].

## 🛠 Tools Used
*   **Programming Language**: Python
*   **Data Analysis**: `pandas` for cleaning, manipulation, and statistical aggregation[cite: 7].
*   **Visualization**: `matplotlib` and `seaborn` for trend and distribution analysis[cite: 7].

## ⚙️ Methodology
1.  **Data Ingestion**: Initial loading of the dataset to evaluate structure and schema[cite: 7].
2.  **Quality Assessment**: Systematic identification of missing values, specifically focusing on `Age` (86 missing) and `Cabin` (327 missing)[cite: 7].
3.  **Exploratory Data Analysis (EDA)**:
    *   Computed central tendencies for numerical variables (e.g., mean age)[cite: 7].
    *   Analyzed feature distribution to determine if data imputation is necessary for modeling[cite: 7].

## 📈 Analysis & Findings
*   **Passenger Age**: The mean passenger age is **30.27 years**, with a wide variance ranging from infancy to 76 years, indicating a diverse age group[cite: 7].
*   **Feature Completeness**: 
    *   The `Cabin` feature is significantly incomplete, with ~78% of data missing[cite: 7].
    *   The `Age` feature has a ~20% missing rate, which is a critical factor for any subsequent predictive modeling[cite: 7].
    *   Minor data cleaning is required for the `Fare` attribute (1 missing entry)[cite: 7].

## 🚀 Results
The analysis provides a clear data dictionary and a roadmap for preprocessing. By identifying the specific missing value patterns and demographic distributions, this project establishes a clean foundation for implementing machine learning algorithms to predict passenger outcomes in future studies.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------


# Bank Marketing Analytics: Driving Subscription Insights (PRODIGY_DS_03)

## 🎯 Objective
The primary objective of this project is to perform a rigorous statistical investigation into customer behavior within a banking environment. By analyzing demographic, behavioral, and macroeconomic datasets, the project aims to identify the specific features that statistically influence a client's decision to subscribe to a term deposit.


## 📊 Data Description
The dataset comprises 4,119 records detailing customer interactions during a direct marketing campaign.
*   **Demographics:** Attributes such as `age`, `job`, `marital status`, and `education`.
*   **Behavioral Features:** Metrics including `duration` (length of last call), `campaign` (contact frequency), and `pdays` (time elapsed since last contact).
*   **Macroeconomic Context:** External indicators including `emp.var.rate`, `cons.price.idx`, and `nr.employed`, which provide insight into the economic climate at the time of contact.
*   **Target Variable:** `deposit` (Binary outcome: 'yes' or 'no').
*   **Data Quality:** The dataset is highly clean with no missing values across all 21 features.
*   

## 🛠 Tools Used
*   **Language:** Python 3.x
*   **Libraries:** 
    *   `pandas` & `numpy`: For data manipulation, numerical computation, and statistical encoding.
    *   `matplotlib` & `seaborn`: For exploratory data analysis and visualization.
*   **Environment:** Jupyter Notebook / VS Code.


## ⚙️ Methodology
1.  **Preprocessing:** Encoded the categorical target variable into a numerical format (`deposit_encoded`) to enable correlation analysis.
2.  **Exploratory Data Analysis (EDA):** Performed descriptive statistics and grouped aggregations to identify conversion rate variations across different customer segments.
3.  **Statistical Modeling:** Calculated Pearson correlation coefficients for all numerical independent variables against the target variable to quantify linear relationships and predictive power.


## 📈 Analysis, Results & Findings

### Core Statistical Drivers
| Feature | Correlation | Insight |
| :--- | :--- | :--- |
| **Duration** | +0.4186 | Strongest positive indicator; longer call engagement is highly correlated with success. |
| **Previous** | +0.2557 | Prior engagement history is a significant positive driver. |
| **Nr. Employed**| -0.3492 | Higher employment rates act as a barrier to new deposit subscriptions. |
| **Pdays** | -0.3320 | Increased time since last contact negatively impacts conversion probability. |

## 🚀 Key Findings
*   **High-Conversion Segments:** The most receptive groups are **Students** (23.2% conversion) and **Retired individuals** (22.9% conversion).
*   **Educational Impact:** Customers holding a **University Degree** demonstrate a higher subscription propensity (13.1%) compared to those with basic education (7.5% - 8.9%).
*   **Engagement Strategy:** The high correlation between `duration` and `deposit` implies that the quality of human interaction during the call is the most vital factor for success.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------


# Sentiment Analysis of Multi-Entity Social Media Data (PRODIGY_DS_04)

## 🎯 Objective
The primary objective of this project was to perform an in-depth exploratory data analysis (EDA) and sentiment classification study on a large-scale social media dataset. The goal was to quantify public sentiment across various entities (brands, games, and technology platforms) to uncover trends in user engagement and brand perception.

## 📊 Data Description
The dataset, `twitter_training.csv`, consists of social media posts associated with various entities[cite: 3].
* **Structure:** The dataset contains four main columns: `ID`, `Entity` (the subject of the post), `Sentiments` (the classification label), and `Contest` (the text content of the post)[cite: 3].
* **Sentiment Categories:** Each post is categorized into one of four labels: *Positive*, *Negative*, *Neutral*, or *Irrelevant*[cite: 3].
* **Dataset Scale:** The dataset is substantial, with several entities represented by approximately 2,400 entries each, allowing for robust statistical evaluation[cite: 3].

## 🛠 Tools & Technologies
The project was executed using Python, ensuring scalability and reproducibility:
* **Pandas:** Used for data ingestion, cleaning, multi-level grouping, and statistical aggregation.
* **Jupyter Notebook:** Employed as the development environment for iterative data exploration.
* **Statistics:** Calculated proportions and distributions to derive normalized insights across the entire dataset[cite: 3].

## ⚙️ Methodology
1. **Data Ingestion:** Loaded the raw data and assigned descriptive column names to facilitate easier manipulation[cite: 3].
2. **Global Sentiment Profiling:** Performed a global frequency analysis to understand the overall polarity of the dataset[cite: 3].
3. **Entity Identification:** Extracted the top 10 most frequently discussed entities to identify key areas of interest within the social media discourse[cite: 3].
4. **Comparative Analysis:** Conducted a cross-tabulation of the top 5 entities to compare how sentiment distributions vary significantly between different brands and products[cite: 3].

## 🔍 Analysis
The analysis revealed significant variance in sentiment depending on the entity:
* **Overall Dataset Sentiment:** Across the entire dataset, *Negative* sentiment is the most prevalent at **30.18%**, followed by *Positive* at **27.89%**, *Neutral* at **24.53%**, and *Irrelevant* at **17.39%**[cite: 3].
* **Brand-Specific Trends:** 
    * **MaddenNFL** shows an overwhelming concentration of *Negative* sentiment (1,710 entries) compared to other categories[cite: 3].
    * **Microsoft** displays a more balanced, "Neutral-leaning" distribution, with *Neutral* being the most frequent sentiment (846 entries)[cite: 3].
    * **LeagueOfLegends** highlights a higher engagement in *Neutral* and *Positive* sentiment compared to the negative-heavy trends observed in other entities[cite: 3].

## 📈 Results & Findings
* **Prevalence of Negativity:** Public discourse in this dataset is skewed toward negativity, with negative posts outnumbering positive ones by nearly 3 percentage points globally[cite: 3].
* **Entity Sensitivity:** Sentiment is highly entity-dependent. For instance, entities like *MaddenNFL* face high negative sentiment ratios, whereas *Microsoft* maintains a more neutral public profile[cite: 3].
* **Actionable Insight:** The disparity in sentiment between entities like *Microsoft* (neutral/balanced) and *MaddenNFL* (negative-dominant) suggests that brand health in this context is heavily linked to the specific entity being discussed, rather than a universal trend across all topics[cite: 3].


---------------------------------------------------------------------------------------------------------------------------------------------------------------


# Road Traffic Accident Severity Analysis (PRODIGY_DS_05)

## 🎯 Project Overview
The objective of this project is to analyze a road traffic accident dataset to understand the primary factors influencing accident severity. By examining variables such as environmental conditions, driver demographics, and vehicle characteristics, this analysis aims to extract actionable insights that could potentially inform road safety improvements.

## 📊 Dataset Description
The dataset consists of **12,316 entries** across **32 features**. It encompasses a wide range of variables, including:
*   **Temporal/Environmental:** Time of accident, day of the week, light conditions, weather conditions, and road surface conditions.
*   **Driver/Vehicle:** Age, gender, educational level, driving experience, vehicle type, and vehicle defects.
*   **Accident Details:** Type of collision, number of vehicles involved, number of casualties, and the primary cause of the accident.
*   **Target Variable:** `Accident_severity` (classified as Slight Injury, Serious Injury, or Fatal injury).

## 🛠 Tools Used
*   **Python:** Primary programming language for data processing and analysis.
*   **Pandas:** Used for data manipulation, cleaning, and aggregation.
*   **Jupyter Notebook:** Used for exploratory data analysis (EDA).

## ⚙️ Methodology
1.  **Data Cleaning:** Evaluated missing values across features such as `Service_year_of_vehicle` and `Defect_of_vehicle`.
2.  **Exploratory Data Analysis (EDA):** Performed univariate and bivariate analysis to determine the frequency distributions and correlations between independent variables and `Accident_severity`.
3.  **Statistical Aggregation:** Calculated total counts and percentage distributions for the target variable to establish a baseline understanding of accident severity.

## 🔍 Analysis & Findings
The analysis of the dataset revealed distinct patterns regarding accident severity:

*   **Severity Distribution:** The vast majority of accidents result in **Slight Injury (84.56%)**, followed by **Serious Injury (14.15%)**, with **Fatal injuries** accounting for a small portion (**1.28%**) of the total recorded incidents.
*   **Prevalent Demographics:** The data indicates that a significant number of drivers involved in accidents fall within the **18-30 age band**, and the majority of recorded drivers are **Male**.
*   **Environmental Factors:** Most accidents occurred under **Daylight** conditions, and the most common road surface condition was **Dry**.
*   **Accident Characteristics:** "Going straight" is the most frequent vehicle movement during accidents, and the most common type of collision is "Vehicle with vehicle collision."

## 🔍 Conclusion
The dataset demonstrates that road safety initiatives might be most effective by focusing on the prevalent drivers (18-30 age band) and the most common accident types (vehicle-to-vehicle collisions). While fatal injuries are statistically rare in this dataset, the high volume of slight injuries suggests a need for consistent adherence to traffic regulations, even in seemingly safe, dry, and well-lit conditions.
