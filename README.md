# 📁 CSV Chunk Uploader & Emailer using Flask
This Flask-based web application allows users to upload large CSV files, split them into chunks (1 million rows per file), and optionally email the resulting files to one or more recipients.

🚀 Features
Upload large .csv files via a simple web interface

Automatically splits files into chunks of 1 million rows each

Retains headers in all chunks

Sends the processed chunks as email attachments to specified recipients

Directory structure and output location can be customized

Useful for data processing, operations, or logistics teams handling large datasets

🛠️ Tech Stack
Python 🐍

Flask 🌐

Pandas 📊

smtplib + email.mime (for sending emails) 📧

HTML (for frontend upload form)

📤 Usage
Upload a .csv file via the web form.

Enter recipient email addresses (comma-separated).

Click "Upload and Send Email".

Processed CSV chunks will be:

Saved in the OUTPUT_FOLDER

Sent as email attachments to the entered recipients

📌 Notes
Default chunk size is 1,000,000 rows – configurable in CHUNK_SIZE.

Output filenames follow the pattern:
Actual_Attempt_Geo_Data_TID_Level_<chunk_number>.csv

You can customize paths, email settings, and output naming as per your use case.

✅ To-Do / Enhancements
 Add progress bar / upload status

 Drag and drop support

 File format validation

 Better error handling and logs

 Dockerize the app for deployment

💡 Example Use Cases
Logistics: Splitting massive geo-TID datasets

Data Ops: Handling file size limits in ERP/email systems

Admins: Distributing processed data to team members via email

📬 Contact
Made with ❤️ by Subhasis Mohanty
Feel free to raise issues or suggestions!
