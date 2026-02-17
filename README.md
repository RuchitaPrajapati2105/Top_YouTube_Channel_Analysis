# 📊 UK YouTubers 2024 – Marketing Collaboration Intelligence
End-to-end Power BI project transforming YouTube metrics into actionable marketing insights.

> **Power BI | Marketing Analytics | Data Storytelling**

### 📌 Project Overview

This repository showcases an end-to-end **Power BI analytics project** designed to support **marketing decision-making** by identifying high-performing UK YouTube creators for potential collaborations in 2024.

The project demonstrates my ability to translate **business requirements into analytical solutions**, apply data quality checks, build engagement-focused KPIs, and communicate insights through an interactive dashboard.

#
### 📁 Dataset

The dataset used in this project was sourced from:

Source: Top 100 UK Youtube Channel Performance Analysis (Kaggle)<br/>
Kaggle – <a href="https://www.kaggle.com/datasets/bhavyadhingra00020/top-100-social-media-influencers-2024-countrywise?resource=download">Dataset Link</a> 🔗<br/>
Topic Of Influence: The niche or category in which the influencer specializes or creates content, such as fashion, beauty, technology, fitness, etc.<br/>
Country: UK<br/>
Year: 2024<br/>
Reach:  The primary social media platform where the influencer is active, such as YouTube.


#
### 🎯 Business Problem

With increasing competition on YouTube, understanding what drives channel growth and engagement is critical.

This project answers key questions such as:

Which categories dominate in subscriber growth?

Is there a relationship between total views and subscriber count?

Which channels demonstrate the highest engagement efficiency?

What patterns exist among top-performing creators?

#
### 🛠️ Tools & Technologies Used

Power BI Desktop – Interactive dashboard creation

Excel / CSV – Data storage

SQL Server – Testing, and analyzing the data

Data Cleaning & Transformation – Power Query

DAX – Calculated measures and KPIs

Data Visualization – Charts, KPIs, Filters, Slicers

#
### 📂 Project Structure
Top_YouTube_Channel_Analysis/ assets        
│                                   
├── datasets/                                    
│   └── top_100_youtube_channels.csv      
│                                       
├── dashboard/                              
│   └── view_top_uk_youtubers_2024.pbix                           
│                     
├── screenshots/                                                    
│   └── dashboard_preview_page1.png   <br>
│   └── dashboard_preview_page2.png                                                                                                  
│                             
└── README.md

#
### 🧮 Metrics Created
The following calculated measures were created in Power BI using DAX:

1. Total Subscribers (M)
    <img width="1126" height="131" alt="Screenshot 2026-02-16 211258" src="https://github.com/user-attachments/assets/65c095c3-5f3e-4a16-ac4c-133641ecce30" />


2. Total Views (B)
    <img width="1123" height="133" alt="Screenshot 2026-02-16 211725" src="https://github.com/user-attachments/assets/2b5f96a1-8174-45e4-9124-e86f0e4547ec" />


4. Total Videos
    <img width="1125" height="90" alt="Screenshot 2026-02-16 211843" src="https://github.com/user-attachments/assets/85e7ac51-cf7d-45fc-93c5-0b94051460ca" />


- **Views per Subscriber** =    
    DIVIDE(
      SUM('view_top_uk_youtubers_2024'[total_views]),
      SUM('view_top_uk_youtubers_2024'[total_subscribers])
    )       

- **Views per Video** =       
    DIVIDE(
      SUM('view_top_uk_youtubers_2024'[total_views]), 
      SUM('view_top_uk_youtubers_2024'[total_videos])
    )

- **Subscribers per Video** =     
    DIVIDE(
      SUM('view_top_uk_youtubers_2024'[total_subscribers]), 
      SUM('view_top_uk_youtubers_2024'[total_videos])
    )

- **Median Views per Video** =    
   MEDIANX(
        VALUES('view_top_uk_youtubers_2024'[channel_name]),
        [Views per Video]
    )


#
### 📊 Dashboard Features

The Power BI dashboard includes:

📈 Total Subscribers & Total Views KPI

📊 Category-wise Channel Distribution

📉 Subscriber vs Views Correlation Analysis

🏆 Top 10 Channels by Subscribers

🎯 Engagement Comparison

🔍 Interactive Filters (Category, Rank, Channel Name)

#
### 🔍 Key Insights

- Entertainment and Music categories dominate the platform.
- High subscriber count does not always guarantee proportional engagement.
- Some mid-ranked channels show stronger engagement efficiency compared to top-ranked channels.
- There is a strong positive correlation between total views and subscriber count.

#
### 📸 Dashboard Preview

Preview - 1
<img width="1279" height="726" alt="dashboard_preview_page1" src="https://github.com/user-attachments/assets/fa3e99c1-7b8f-4e05-9122-b55d50785067" /><br/>

Preview - 2
<img width="1278" height="728" alt="dashboard_preview_page2" src="https://github.com/user-attachments/assets/ac7b4975-76c3-4388-9582-812e3c2f792f" /><br/>

#
### 💡 Skills Demonstrated

- Data Cleaning & Preparation

- Business Problem Framing

- KPI Development

- DAX Measures

- Data Storytelling

- Insight Generation

- Dashboard Design Best Practices

#
### 🚀 How to Use

- Download the .pbix file from the dashboard folder.

- Open using Power BI Desktop.

- Interact with filters and visuals to explore insights.

#
### 📈 Future Improvements

- Add engagement rate calculation (Likes / Views)
- Add time-series growth trend (if historical data available)
- Integrate API-based real-time data
- Deploy dashboard to Power BI Service

#
### 👩‍💻 About Me

I am a Data Analyst with experience in transforming data into actionable insights using Power BI, Excel, and SQL. I focus on building business-driven dashboards that support decision-making.

📩 Open to Data Analyst opportunities in Canada<br/>
🔗 Connect with me on <a href="https://www.linkedin.com/in/ruchitaprajapati/" style="color:orange;">LinkedIn</a> | <a href="mailto:ruchiprajapati2105@outlook.com" style="color:orange;">E-mail</a> <br/>
📂 Explore more projects on <a href="https://github.com/RuchitaPrajapati2105/" target="_blank">my GitHub</a>
