# Customer Satisfaction Feedback Automation

I built this n8n workflow to collect customer feedback after an order is completed, analyze the customer's rating and comment, and notify the team when follow-up is needed.

<img width="414" height="237" alt="Customer Satisfaction workflow demo" src="https://github.com/user-attachments/assets/27324f0b-e3d9-4ae9-bd1f-31fb5d1407a4" />

## How it works

1. The workflow checks for completed orders on a schedule.
2. It sends the customer an email survey asking for a rating from 1 to 10 and feedback.
3. When a response is added to Google Sheets, Gemini analyzes the rating and comment.
4. The response is classified as satisfied, neutral, or dissatisfied.
5. If follow-up is needed, the team receives a Telegram notification.

## Technologies

n8n, Google Sheets, Gmail, Google Gemini, Telegram, and JavaScript.

## Setup

Import [workflow.json](./workflow.json) into n8n, connect Google Sheets, Gmail, Gemini, and Telegram, then select your orders sheet and feedback responses sheet.
