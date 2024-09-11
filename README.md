![pexels-pixabay-236937 new](https://github.com/user-attachments/assets/87105ee3-14f1-4d70-80fc-0b2cc3fda9cb)

# 120 Years of Olympic History Analysis

In this project, I analyzed the historical data from the modern Olympic Games to identify trends and patterns in athlete participation, country representation, and overall performance across different editions of the Olympics. The goal of this analysis was to gain a deeper understanding of how the participation of athletes and countries has evolved over the years.

# Dataset

The "120 Years of Olympic History" dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results?select=noc_regions.csv). It contains comprehensive historical data on the modern Olympic Games, spanning from the inaugural Athens 1896 Olympics to Rio 2016.

Each row in the dataset represents an individual athlete competing in a specific event and includes details such as the athlete’s name, age, sex, country, medal, and more.

# Data Pre-processing and Cleaning

After loading the dataset into Excel, I utilized Power Query to clean and preprocess the data:

* **Removed Unnecessary Columns:** Deleted columns like "ID" and "NOC" that were not relevant to the analysis.
* **Corrected Data Types:** Converted data types for certain columns (e.g., changing integer columns incorrectly marked as strings).
* **Feature Engineering:** Created an additional "Edition" column to uniquely identify each Olympic session by city.

To handle missing values in the age, height, and weight columns, I filled them with the respective mean values, grouped by the event category, as some events have specific combinations for these attributes. Below is an example formula used to fill null values in the "Age" column:

![Age_filled](https://github.com/user-attachments/assets/7f5e0189-f339-423c-9452-5d48ef4608a7)


Similar methods were applied to the weight and height columns.

Finally, I have below a sample of stock uncleaned data, followed by the cleaned data.

Uncleaned Data:
![Uncleaned Data](https://github.com/user-attachments/assets/3692fca3-5d48-4d83-9495-a0d66b1daaec)

Cleaned Data:
![Cleaned Dataset first 20 rows](https://github.com/user-attachments/assets/ec381d8b-ad08-43d8-8be3-1c2aa44b05cf)


# Exploratory Data Analysis (EDA)

Using pivot tables in Excel, I explored the following aspects:

* Trends in athlete and country participation over time.

* Distribution of age, height, and weight among athletes.

![Age](https://github.com/user-attachments/assets/38c76bce-b3a1-47e0-9843-17749cb250fc)

![Height](https://github.com/user-attachments/assets/e15d8afd-4b4e-4e26-b252-68f81f6b9062)

![Weight](https://github.com/user-attachments/assets/213bbca4-0a1e-4c61-a673-b1ad36698f09)

* Top athletes and countries based on the number of medals won.

* The ratio of male to female participants over the years.

![Gender](https://github.com/user-attachments/assets/c6e02106-18d7-41a7-bcb3-063ad3fe6227)

* Cities that hosted the most Olympic editions.

# Dashboard Creation
I created a comprehensive dashboard to provide an overview of the analysis:

![Final Dashboard](https://github.com/user-attachments/assets/b4c09512-baf5-4362-bf22-8d2050510f73)


* **Key Performance Indicators (KPIs):** Measures for total participants, total medals, and total sports were added to highlight overall performance.

* **Filters for Multilevel Views:**
  * *Season:* To differentiate between the Summer and Winter Olympics.
  * *Gender:* To compare participation and performance between male and female athletes.
  * *Year:* To analyze trends over different periods.

Filters in action:
![Dashboard with Filters](https://github.com/user-attachments/assets/f8437103-bd9a-4656-9143-9b16669a221a)
