# Inventory Reorder Management

An n8n workflow that compares inventory levels with sales history, estimates remaining stock coverage, and asks AI to recommend reorder quantities and urgency.

## How it works

1. The workflow reads inventory and sales records from Google Sheets.
2. JavaScript calculates product-level sales indicators and stock coverage.
3. An AI agent proposes a reorder quantity, urgency, and reasoning.
4. The result is saved to a spreadsheet and sent as a Telegram notification.

## Technologies

- n8n
- Google Sheets
- AI Agent
- Anthropic Chat Model
- JavaScript
- Telegram

## Setup

1. Import workflow.json into n8n.
2. Configure Google Sheets, AI model, and Telegram credentials.
3. Connect your inventory and sales sheets and map their columns to the workflow fields.
4. Test using sample inventory and sales records before enabling the schedule.

## Notes

This repository contains the exported n8n workflow. Configure your own credentials and integrations in n8n before running it.
