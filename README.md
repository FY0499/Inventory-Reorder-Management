# Inventory Reorder Management

I built this n8n workflow to monitor inventory levels using stock and sales data, estimate how many days remain before a product runs out, and get AI recommendations for reorder quantities.

<img width="886" height="265" alt="Inventory Reorder Management workflow demo" src="https://github.com/user-attachments/assets/b8bfa865-4f4b-44e2-ab1a-77dd89c6eed8" />

## How it works

1. The workflow reads inventory records and sales records from Google Sheets on a schedule.
2. JavaScript matches sales to each product and calculates the total quantity sold, average daily sales, and estimated days until stockout.
3. An AI agent reviews the product information and recommends a reorder quantity, urgency level, and reason.
4. The recommendation is saved to Google Sheets.
5. A Telegram message is sent with the product details and suggested reorder quantity.

## Main features

- Automatic inventory and sales data checking.
- Average daily sales calculation.
- Estimated days until stockout.
- AI-suggested reorder quantity and urgency.
- Google Sheets records and Telegram notifications.

## Technologies

n8n, Google Sheets, Anthropic Chat Model, AI Agent, JavaScript, and Telegram.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Google Sheets, Anthropic, and Telegram credentials, then connect your inventory and sales sheets and make sure the SKU and quantity fields match the workflow.
