# DSA210-FALL-24-PROJECT

# Coffee Consumption Patterns on Campus

The aim of this project is to conduct a comprehensive analysis of my coffee purchasing habits during the current semester. This analysis is based on transaction data obtained from my bank account, focusing on five coffee shops located within my university campus: Starbucks, Espressolab, Coffy, Fasshane and Simit Sarayı.

Through this project, I seek to identify patterns in my spending behavior, such as the frequency and timing of purchases at each coffee shop. Additionally, I aim to explore correlations between these purchasing habits and external factors, including exam periods and the locations of my classes. By gaining insights into how these factors influence my coffee shop preferences, I hope to better understand the role of convenience, academic stress, and schedule in shaping my consumption choices.

The results of this analysis could offer meaningful observations about how personal routines and environmental factors impact daily spending behaviors, particularly in a campus setting where options are limited to specific vendors.

- Code related to my project can be found in
- The presentation can be found in https://docs.google.com/presentation/d/1xQR5WUnsheCSNZoUFfqBxDouofJyHl7i92n78sVOTuo/edit?usp=sharing

# Data Collection and Preprocessing

# a. Bank Account Data
Source: Bank transaction statements.
Extraction:
- Retrieved relevant transaction details such as date, time, and description.
- Filtered transactions that corresponded to coffee shop purchases using regex patterns.
# b. Academic Calendar Data
Source: Google Calendar exported as a CSV file.
Extraction:
- Parsed lesson/exam schedules including date, time, lesson name, and location.
- Used the structure of rows in the calendar file to correctly extract relevant information.

In the preprocessing phase, I ensured that the data was clean, consistent, and ready for analysis. 

For the bank account data, I used regular expressions to identify coffee shop purchases from transaction descriptions, filtered out irrelevant rows, and standardized the dates to a uniform format (DD/MM/YYYY). 

For the academic calendar data, I extracted meaningful rows from its multi-row structure, parsed the date, time, lesson name, and location, and removed any rows with missing or invalid values. I standardized column names across the datasets to maintain clarity. Then, I integrated the datasets by merging the bank account data and academic calendar data based on matching dates. Additionally, I mapped lesson locations to corresponding coffee shops using predefined rules and appended manually entered exam data to the academic calendar dataset. 

Finally, I organized the processed data into structured CSV files with relevant columns for easy analysis.

# Exploratory Data Analysis (EDA)

For the exploratory data analysis (EDA) in my project, I utilized a combination of tools to uncover patterns, trends, and relationships in the data. 

Python served as a primary tool for data manipulation and visualization, with libraries such as pandas for data handling and matplotlib for creating insightful visualizations. 

Additionally, Excel played a significant role in comparing datasets and analyzing results, as I used its pivot tables and filtering features to examine specific trends and correlations, as well as its built-in charting tools to create quick visual representations of the data. 

To further enhance the visual analysis, I used Desmos to draw and explore graphs interactively, allowing for a more intuitive understanding of certain patterns and relationships in the data. 

And I also employed Tabula to extract and preprocess data from PDF files, making it easier to integrate and analyze structured information. 

# Key Findings

# 1.Mismatch Between Academic Program and Coffee Shop Preferences:
- Based on the analysis of my academic program, Simit Sarayı should align most with my schedule due to its proximity to the majority of my lesson locations.
- However, my actual coffee shop preferences indicate that I predominantly shop at Starbucks.

# 2.Academic Schedule's Influence on Coffee Purchases:
- There were 25 matches out of 55 coffee shopping records, where the coffee shop aligned with my academic schedule.

# 3.Starbucks as a Preferred Choice:
- Despite the academic schedule favoring Simit Sarayı, Starbucks remains my most visited coffee shop, suggesting other factors such as personal preference or convenience might also play a role.

# Future Work

For future work, this project can be expanded by incorporating additional factors influencing coffee shop preferences, such as proximity to social activities, menu options, waiting times, and promotions. A detailed time-series analysis could be conducted to study how coffee purchase patterns evolve over different semesters or during exam-heavy weeks. Combining quantitative data with qualitative insights from surveys or interviews could provide a deeper understanding of why certain coffee shops are preferred. 

Integration of more data sources, such as walking distances, weather conditions, or crowd density at coffee shops, would refine the analysis further. Predictive models using machine learning techniques could be developed to forecast coffee shop preferences based on academic schedules, time, and other variables. A recommendation system could also be designed to suggest the most convenient coffee shop based on individual preferences and academic schedules. 

Additionally, extending the study to include data from peers could help identify broader patterns or differences among similar academic routines, while a longitudinal study could track changes in preferences over time. From this project, I have already improved my skills in data collection, preprocessing, and visualization, as well as gained a deeper understanding of how personal routines affect decision-making. In the future, these insights could be leveraged for personal efficiency, cost-saving strategies, and even creating predictive tools or dashboards that could be shared or monetized for broader use.

# Conclusion 
