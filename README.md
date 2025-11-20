# LuxeTrend Fashion – Paid Marketing Campaign Analysis

*Multi-channel advertising ROI analysis using SQL – Facebook, Pinterest, Google Ads, TikTok | 150,000+ data | 9,000+ rows | £1.2M spend analyzed*

## 📁 Business Context & Problem Statement

LuxeTrend Fashion is a growing UK online fashion brand that invested heavily in paid advertising throughout 2023. The marketing team needed clear answers to:

- Which campaigns, channels, devices, and cities deliver the best return on investment?
- Where should we reallocate budget for 2024?
- Are certain ad creatives ("Collection" vs "Discount") performing significantly better?
- Is there seasonality or device preference we are missing?

This project answers all of these questions using only SQL on a 9k+ dataset.

## 📅 Dataset Overview

- **Source**: Internal ad platform export (Facebook Ads Manager, Google Ads, Pinterest, TikTok)
- **Time period**: 01/03/2023 – 30/11/2023
- **Rows**: ~9,500+ daily records
- **Key columns**:
  - Campaign (Spring, Summer, Fall, Winter)
  - Date, City_Location, Channel, Device (Desktop/Mobile/Tablet), Ad (Collection/Discount/etc.)
  - Impressions, Clicks, CTR, Daily_Avg_CPC, Spend_GBP
  - Conversions, Total_conversion_value_GBP
  - Likes_Reactions, Shares, Comments

## 💡 Key Insights & Business Recommendations

| Insight | Business Recommendation | Expected Impact |
| ------- | ------------------------- | --------------- |
| Fall campaign delivered 18.03% higher conversions vs Spring | Reallocate 30–40% of Spring budget to Fall/Winter | +25–35% total conversions |
| Pinterest **Desktop** is the ROI champion (avg ~468%) | Scale Pinterest Desktop aggressively ("Discount" creatives) | 4–5× ROAS, highest profit channel |
| **Desktop** converts at 23.99% vs Mobile 20.42% | Keep strong desktop bidding & creatives; don’t go “mobile-only” | Higher revenue per click |
| Manchester & London dominate engagement; Birmingham/Glasgow win on pure conversion rate | Awareness budget → Manchester/London<br>Conversion budget → Birmingham/Glasgow | Optimised funnel performance |
| "Discount" ads crush "Collection" ads on Pinterest | Shift creative focus to discount-led messaging on Pinterest & test on TikTok | Faster inventory turnover, higher margins |
| Clear Q4 spike (Sep–Nov) | Front-load budget from mid-August onwards | Capture Black Friday buildup early |

## 📊 Visualizations

![Top Performing Campaign  
![ROI by Channel & Device](visualizations/02_roi_by_channel.png)  
Highest ROI: Pinterest Mobile  

![Conversions by Device](visualizations/03_conversions_by_device.png)  
Mobile dominates  

![Seasonal Trend](visualizations/04_seasonal_trends.png)  
Clear Q4 spike  

(You can create these quickly in Power BI, Tableau Public, or even Google Sheets → export as PNG)

## SQL Queries Included

All queries are fully commented in `sql/04_analysis_queries.sql`

1. Top campaign by impressions/clicks/conversions  
2. Average CPC & CTR per campaign  
3. Channel with highest profit (Total_value – Spend)  
4. Performance breakdown by channel  
5. Top cities by engagement rate  
6. Conversion rate by city and by device  
7. Best performing individual ads (engagement + conversions)  
8. ROI matrix by Campaign × Channel × Device  
9. Spend vs Conversion Value correlation  
10. Daily trend analysis (seasonality)

## 💼 Tool Kit

- MySQL
- CSV → SQL import
- Visualization in Excel
