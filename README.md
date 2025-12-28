📩 Serverless Contact Form Using AWS Lambda

A fully serverless contact form solution that collects user messages and stores them securely in Amazon DynamoDB — no servers needed!

🚀 Project Overview

This project solves the challenge of handling form submissions without a traditional backend.
By using AWS services like API Gateway, Lambda, and DynamoDB, form data is processed and saved seamlessly in the cloud.

🧰 Tech Stack
Component	Service Used
Backend	AWS Lambda (Node.js/Python)
API	Amazon API Gateway
Database	Amazon DynamoDB
IAM	Role for Lambda execution and DynamoDB access
Frontend	HTML Contact Form
✨ Features

✔ Send messages from a simple web form
✔ Data stored automatically in DynamoDB
✔ No server administration or maintenance
✔ Scalable and pay-per-use model
✔ Secure IAM role permissions

📌 Architecture Flow

User → Contact Form → API Gateway → Lambda → DynamoDB

🏗 AWS Setup Steps

1️⃣ Create a DynamoDB Table

Table Name: ContactForm

Primary Key: email (String)

2️⃣ Create a Lambda Function

Runtime: Node.js/Python

Add permissions:

AmazonDynamoDBFullAccess

AWSLambdaBasicExecutionRole

3️⃣ Configure API Gateway

Add a POST route

Integrate with Lambda

Deploy the API

Copy the Invoke URL

4️⃣ Update your HTML Form

Replace API URL in fetch/AJAX or form submission

🧪 Testing the Form

Open your HTML page in the browser

Enter name, email, and message

Submit ➝ Check DynamoDB table to see stored item ✔

📸 Screenshots

/screenshots/n1.png
/screenshots/n2.png
/screenshots/n3.png
/screenshots/n4.png
/screenshots/n5.png


📂 Project Structure
├─ index.html
├─ lambda_function.py (or index.js)
└─ README.md

🔒 Security Best Practices

🔹 Validate email and message format
🔹 Add CORS restrictions
🔹 Apply least-privilege IAM access
🔹 Enable CloudWatch logs for monitoring

🎯 Outcome

A production-ready serverless backend that captures user messages efficiently and can scale without limits.

📚 Future Enhancements

Email notifications via Amazon SES

reCAPTCHA for bot protection

UI improvements using CSS/Bootstrap

Analytics with CloudWatch
