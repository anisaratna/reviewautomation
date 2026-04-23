# AI-Powered Competitor Intelligence & Customer Insights Automation

## Project Overview
This project demonstrates an end-to-end AI automation pipeline built for the beauty industry. It automates the collection of customer reviews and utilizes **Large Language Models (Llama 3.3 70B)** to transform messy, informal Indonesian text into structured Business Intelligence.

## Key Challenges & Solutions
* **Data Scale:** Scraped **400+ real-world reviews** from Female Daily.
* **API Rate Limits:** Developed a custom **Batch Processing System** with automated retries and a **Checkpoint/Resume** mechanism to handle API constraints gracefully.
* **Informal Language:** Engineered prompts to accurately interpret Indonesian "slang" and informal beauty terminology.

## Tech Stack
* **Engine:** Python, BeautifulSoup4
* **AI:** Llama 3.3 70B (via Groq API)
* **Logic:** Few-Shot Prompting, Chain-of-Thought (CoT), JSON Output
* **Analytics:** Pandas, Seaborn, Matplotlib

## Deep-Dive Analytics
Unlike standard sentiment analysis, this project explores the correlation between **Skin Types** and **Product Satisfaction**.

### Key Finding: The "Combination Skin" Anomaly
While the product maintains an overall **89% positive sentiment**, the analysis revealed that **Combination Skin** users show the highest variance in satisfaction. 
* *Hypothesis:* The current gel formula might be optimal for the T-zone but lacks sufficient hydration for the dryer U-zone.

<img width="1432" height="586" alt="gambar" src="https://github.com/user-attachments/assets/82084023-4c43-42cc-8bcc-b310ead20deb" />

## AI-Generated Executive Recommendations (R&D Roadmap)
Based on the automated thematic clustering of 400 reviews:
1. **Hydration Boost:** Develop a "Combination Skin" specific variant with balanced humectants.
2. **Formula Transparency:** Address concerns about "eye stinging" mentioned in 7% of negative reviews by optimizing the preservative system.

## Repository Structure
* `Beauty_Review_LLM.ipynb`: Contains the full pipeline from scraping to LLM processing.
* `azarine_reviews_large.csv `: Raw datasets.
* `ai_analysis_results.cs `: Processed datasets.
* `requirements.txt`: Necessary libraries 
