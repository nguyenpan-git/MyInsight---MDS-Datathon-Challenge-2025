# ZaloPay Bot Fraud Detection - MyInsight Datathon 2025

| Thành viên         |
|------------------- |
| Huỳnh Bảo Sang     |
| Nguyễn Văn Phúc An |
| Võ Nhật Tiến       |

## Project Overview
This repository contains the solution for the **MyInsight MDS Datathon Challenge 2025 (1st Runner-Up)**. The project focuses on detecting and mitigating bot-driven promotion abuse in ZaloPay's e-wallet campaigns, addressing a potential revenue loss of 1.18 billion VND.

## Key Highlights
* **Data Processing:** Analyzed 7 interconnected datasets covering over 864K+ users to trace and identify promotion abuse patterns.
* **Risk Scoring Model:** Developed a real-time Rule-based Scoring System (Heuristic Model) extracting quantitative features for 5 abnormal behavioral patterns (e.g., transaction speed, spamming, duplicate IPs).
* **Optimization:** Fine-tuned the detection threshold using the Gini index (0.82) to balance Precision and Recall, achieving an optimal 0.13% False Positive Rate.
* **Strategic Solutions:** Proposed proactive defense mechanisms including hidden honeypot codes and gamified CAPTCHA to block bots without degrading genuine user experience.

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
