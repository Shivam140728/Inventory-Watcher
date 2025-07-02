📦 Project Name:
Inventory Watcher
Smart Product Alerting & Reporting System using Google Apps Script

📄 Description:
Inventory Watcher automates your inventory analysis using Google Sheets + Apps Script. It fetches product data from an API, filters best-performing items, sends email alerts, generates downloadable reports, and builds a live dashboard with charts and KPIs — helping teams stay informed and act faster.

🚀 Key Features:
✅ 1. 📩 Email Alert for Best Products
Automatically emails the top 5 best products daily.

Product details include title, price, discount %, and rating.

✅ 2. 📄 PDF/CSV Export of Best Products
Exports selected top products into a CSV file.

Files are stored in Google Drive for backup and sharing.

✅ 3. 📊 Inventory Dashboard
Dynamic dashboard in Google Sheets (Dashboard tab) showing:

🔢 Total Products

💸 Average Price

🌟 Average Rating

❗ Low Stock Warnings

📈 Discount vs Rating Chart

📊 Column Chart for Product Ratings

✅ 4. Low Stock Highlighting
Highlights products with stock below threshold (e.g., < 10) in red/pink for quick action.

🔧 Technologies Used:
Google Apps Script

Google Sheets

DummyJSON API (https://dummyjson.com/products)

MailApp, DriveApp, ChartBuilder

🛠 How It Works:
Fetch API Data → Loads product data into Sheet1

Filter Best Products → Based on rating >= 4 & discount <= 2%

Update Best_Products Sheet → Highlights & stores best items

Email Alert → Sends summary of top 5 items

CSV Export → Saves best products to Drive

Dashboard → Visualizes KPIs and discount-rating trends

📧 Sample Email Output:
yaml
Copy
Edit
🛒 Today's Best Products

Calvin Klein CK One | Price: $49.99 | Discount: 1.89% | Rating: 4.37
Cucumber             | Price: $1.49  | Discount: 0.16% | Rating: 4.07
...
📈 Sample KPIs in Dashboard:
Metric	Value
Total Products	30
Avg. Price	₹499.20
Avg. Rating	4.25

Includes:

🔵 Scatter Plot: Discount vs Rating

🟩 Column Chart: Product Ratings

📥 Output Files:
📧 Email To: shivam.kumar140728@gmail.com

📄 CSV File: "Best Products List.csv" in Google Drive

📊 Visuals: In Dashboard sheet

🔄 Recommended Triggers:
Daily at 9:00 AM → Run APIData()

Weekly → Run CreateDashboard()

📈 Possible Future Enhancements:
🔔 WhatsApp Alerts via Twilio

📅 Calendar Integration for stock restock reminders

📤 PDF Export of visual dashboard

🧮 Sales trend forecasting
