# Restaurant-Chatbot-using-AWS-Lex-Lambda-and-DynamoDB

# 🍴 AWS Restaurant Chatbot

An AI-powered chatbot that allows users to order food items and stores their orders in AWS DynamoDB using Lex and Lambda.

## 🚀 Tech Stack
- **Amazon Lex V2** – Chat interface
- **AWS Lambda (Python 3.11)** – Logic and integration
- **Amazon DynamoDB** – NoSQL data storage
- **Amazon CloudWatch** – Logging and monitoring
- **AWS IAM** – Access control

## 🧩 Architecture
1. User sends message → Lex detects intent.
2. Lex triggers Lambda → Lambda processes data.
3. Order data is saved to DynamoDB.
4. Response is sent back to user.

## 🗃️ DynamoDB Schema
| Key | Type | Description |
|-----|------|-------------|
| Intent | String | Partition key |
| CustomerName | String | Customer name |
| FoodItem | String | Ordered item |
| Quantity | Number | Item quantity |
| Message | String | Confirmation message |

## 📜 Lambda Function
Written in Python, handles Lex input, inserts data into DynamoDB, and returns response.

## 📈 Features
✅ Serverless architecture  
✅ Secure IAM-based access  
✅ CloudWatch monitoring  
✅ Scalable and easy to extend  

---
