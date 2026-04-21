# n8n-lead-generation-agent
Autonomous B2B lead generation agent using n8n, Apify, and Firecrawl. Extracts business data, emails, and social media from Google Maps.

---

## 🚀 What does this system do?

| Step | Description |
|:---|:---|
| **1** | Reads queries from Google Sheets (e.g., "dental clinics Madrid") |
| **2** | Launches an Apify job to scrape Google Places |
| **3** | Waits for the job to complete and fetches results |
| **4** | For each business with a website, extracts the full HTML |
| **5** | Uses JavaScript and regex to extract: emails, LinkedIn, Facebook, Instagram, Twitter |
| **6** | Saves enriched data to Google Sheets |
| **7** | Marks the query as processed and moves to the next one |

---

## 🛠️ Technologies Used

| Technology | Purpose |
|:---|:---|
| **n8n** | Workflow orchestration |
| **Apify** | Google Places scraping |
| **Firecrawl** | Website HTML extraction |
| **JavaScript (Regex)** | Email and social media extraction |
| **Google Sheets API** | Lead storage and query management |

---

## 📈 Key Results

- ✅ **Batch processing** to avoid API rate limits
- ✅ **Email extraction** with false positive filtering
- ✅ **Social media detection**: LinkedIn, Facebook, Instagram, Twitter
- ✅ **Scalable** to thousands of queries with no manual intervention
- ✅ **Autonomous**: scheduled or manual execution

---

## 🎯 Real Use Case

A marketing agency needs 500 qualified leads for a campaign. Instead of manual searching, this system processes queries automatically and delivers ready-to-use data in a spreadsheet.

---

## 📦 Installation & Setup

1. Clone this repository
2. Import the JSON workflow into your n8n instance
3. Configure credentials:
   - Apify API Key
   - Firecrawl API Key
   - Google Sheets OAuth2
4. Prepare your Google Sheet with queries (columns: Query, Location)
5. Activate the workflow and run it

---

## 📸 Screenshots

*[Add images of the workflow and results here]*

---

## 👨‍💻 Author

**Alejandro Peralta**  
Process Automation Specialist  
[GitHub](https://github.com/yourusername) | [LinkedIn](https://linkedin.com/in/yourusername) | [Email](mailto:alejandro@orbisautomations.com)

---

## ⭐ If you like this project, give it a star!
