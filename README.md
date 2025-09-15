# EventBot 🎉🤖

EventBot is an **Amazon Lex V2 chatbot** designed to help users seamlessly book events.  
It collects event details like **event type, location, attendees, accommodation days, client name, and contact information**. The bot uses **AWS Lambda** for slot validation and fulfillment to ensure accurate bookings.  

---

## 🚀 Features
- Conversational **event booking assistant**  
- Collects key event details:
  - EventType  
  - Location  
  - AttendeesCount  
  - AccommodationDays  
  - ClientName  
  - PhoneNumber  
- **Slot validation** (e.g., ensuring valid number of guests)  
- **Confirmation flow** before finalizing booking  
- Lambda-powered **fulfillment messages**  

---

## 📂 Repository Structure
EventBot/
│── bot-definition/ # Exported JSON/ZIP files from Amazon Lex
│── lambda/ # Lambda function code for slot validation/fulfillment
│ └── lambda_function.py
│── docs/ # Documentation, design notes, flow diagrams
│── README.md # This file


---

## 🛠️ Setup & Usage
 1. Clone the repository  
bash

git clone https://github.com/your-username/EventBot.git
cd EventBot
---
2. Import the bot into Amazon Lex V2

Go to the Lex V2 Console

Choose Import and upload the bot-definition/ file (JSON or ZIP)

3. Deploy the Lambda function

Go to AWS Lambda Console

Create a new function (Python 3.9 or higher)

Copy the code from lambda/lambda_function.py

Attach the Lambda function to your Lex bot

4. Build and test the bot

In Lex console, build your bot

Test it using the test window or connect it to Amazon Connect / a web client
