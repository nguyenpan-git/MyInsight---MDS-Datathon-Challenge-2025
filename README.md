# ZaloPay Bot Fraud Detection - MyInsight Datathon 2025

| Thành viên         |
|------------------- |
| Huỳnh Bảo Sang     |
| Nguyễn Văn Phúc An |
| Võ Nhật Tiến       |

## Project Overview
This repository contains the solution for the **MyInsight MDS Datathon Challenge 2025 (1st Runner-Up)**. The project focuses on detecting and mitigating bot-driven promotion abuse in ZaloPay's e-wallet campaigns, addressing a potential revenue loss of 1.18 billion VND.

## Key Highlights
* **Data Analysis & Processing:** Processed and cleaned an interconnected dataset of 7 tables involving over 864,000 users , isolating bot-driven promotion abuse behaviors that caused a financial loss of 1.18 billion VND for the business.
* **Risk Detection Modeling:** Engineered features for 5 abnormal behaviors (transaction speed, repeated amounts, campaign spamming, etc.) to build a real-time user risk scoring system.
* **Quantitative Optimization:** Applied the Gini index (achieving 0.82) to fine-tune the detection threshold, balancing Precision and Recall, and maintaining an optimal false positive rate (FPR) of 0.13%.
* **Product-led Solutions:** Designed proactive defense mechanisms, including hidden honeypot codes and gamified CAPTCHA verification via Minigames , effectively blocking automated bots without impacting the genuine user experience.

## MODEL USED IN THE CODE
* The model implemented in the provided code is a Rule-based Scoring System (Heuristic Model).
* This system does not learn from data autonomously like traditional Machine Learning; instead, it operates on defined business rules:
  * Feature extraction based on business logic for 5 specific risk criteria.
  * Assigning static weighted scores (ranging from 1 to 8 points) for varying levels of user violations.
  * Aggregating the scores (total_score) and establishing a classification threshold to make decisions.
  * Applying Machine Learning evaluation metrics (Gini Index, Confusion Matrix) to identify the optimal cut-off point at 9.

## Repository Structure
* `Data/`: Contains the sample/masked datasets used for analysis. *(Note: Full raw data is hosted externally due to size limits).*
* `myInsight_V3_AE66_Code/`: Python source code for EDA, feature engineering, and building the scoring model.
* `myInsight_V3_AE66_Dashboard.pbix`: Power BI dashboard for interactive data visualization. 
* `myInsight_V3_AE66_Report.pdf`: Comprehensive slide deck detailing the business problem, methodology, and recommendations.
* `result.xlsx`: The final output file containing user risk scores and fraud classification flags.



* ## External Assets
Due to GitHub's file size limitations, the raw datasets and the interactive Power BI file are hosted securely on Google Drive.

* 🔗 **[Raw Data Folder (Google Drive)]([DÁN_LINK_THƯ_MỤC_DATA_VÀO_ĐÂY](https://drive.google.com/drive/folders/1fr9yWn04LT8iZtEeV8fpg_nnTmU0IEqu?usp=drive_link))**: Contains the original masked CSV datasets.
* 🔗 **[Power BI Dashboard (Google Drive)]([DÁN_LINK_FILE_PBIX_VÀO_ĐÂY](https://drive.google.com/file/d/1XXidE9SaMlfab4X3i2IjsvwnhaIKAqcr/view?usp=sharing))**: The `.pbix` file for interactive data visualization.
