📦 TopPick: Best Product Alert
TopPick is a Google Apps Script-based automation tool that fetches product data from a public API, filters the best-performing products based on customizable business rules (discount and rating), and sends a daily email alert with the top products. This project is ideal for e-commerce teams, data analysts, or inventory managers who want to stay updated on product performance trends.

🚀 Features
🔄 Fetches product data from the DummyJSON Products API

📊 Filters best products based on:

Rating ≥ 4

Discount ≤ 2%

✅ Stores full product list in a Google Sheet (Sheet1)

🌟 Writes filtered products to another sheet (Best_Products) with formatting

💬 Sends automated email with the top products summary

🖌️ Highlights best products in green

🕐 Supports daily automation using triggers

🧠 Logic Criteria
To be marked as a “Top Pick”, a product must satisfy:

Rating ≥ 4

Discount ≤ 2%

These rules can be adjusted in the script to match your business needs.

📁 Sheet Structure
Sheet1 – All Products
Title	Price	Discount	Rating	Stock
All fetched product data from API				

Best_Products – Filtered Products
Title	Price	Discount	Rating	Stock
Only the best products (green highlighted)				

📧 Email Output Example
yaml
Copy
Edit
Here are today's best products:

📦 iPhone 9 | Price: ₹549 | Discount: 1.2% | Rating: 4.69 | Stock: 34  
📦 MacBook Pro | Price: ₹1749 | Discount: 2% | Rating: 4.5 | Stock: 12  
...
🔧 Setup Instructions
Open Google Sheets.

Go to Extensions > Apps Script.

Paste the full code into the script editor.

Create two sheets: Sheet1 and Best_Products.

Replace the email address in the code (MailApp.sendEmail) with your own.

(Optional) Set a time-driven trigger:

Go to ⏰ Triggers in Apps Script

Select function APIData

Choose "Time-driven" > "Day timer" > 9:00 AM (or any time)

💡 Customization Ideas
Add cost price and calculate profit margin

Highlight low-stock products in red

Send product data as PDF or CSV attachment

Add charts and visual KPIs in a third sheet

📚 Tech Used
Google Apps Script (JavaScript)

Google Sheets

MailApp Service

Public API: DummyJSON Products

🙋‍♂️ Author
Shivam Kumar
Data Analyst | Google Apps Script Enthusiast
📧 shivam.kumar140728@gmail.com

