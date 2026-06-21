# AI Expense Tracking Agent

## Overview

The AI Expense Tracking Agent is an intelligent financial assistant designed to automate expense tracking, record management, and financial monitoring through a conversational interface. Instead of manually updating spreadsheets or financial systems, users can simply communicate with the agent through Telegram using natural language.

The system leverages OpenAI, n8n, Google Sheets, Gmail, and Telegram to process expense information, maintain records, provide updates, and notify stakeholders when significant expenses require attention.

---

## Problem Statement

Many individuals and businesses still track expenses manually using spreadsheets or accounting tools that require repetitive data entry. This often leads to:

* Inconsistent record keeping
* Time-consuming manual updates
* Delayed financial reporting
* Poor visibility into spending patterns
* Missed notifications for significant expenses

The objective of this project was to create an AI-powered assistant capable of managing expenses through natural conversation while automating financial record keeping and reporting.

---

## Solution

The AI Expense Tracking Agent enables users to:

* Log expenses through Telegram
* Retrieve existing expense records
* Update previously recorded expenses
* Receive instant confirmations
* Trigger management alerts for important transactions
* Maintain context across conversations using memory

The result is a streamlined, conversational expense management system that reduces manual administrative work and improves financial visibility.

---

## Workflow Architecture

### 1. User Interaction

The workflow begins when a user sends a message through Telegram.

Example:

```text
I spent $150 on fuel today.
```

The message acts as the trigger for the automation.

---

### 2. AI Processing

The message is passed to an OpenAI-powered Expense Tracking Agent.

The AI agent:

* Interprets user intent
* Extracts expense details
* Identifies categories
* Determines required actions
* Structures data for storage

Example extraction:

```json
{
  "amount": 150,
  "category": "Fuel",
  "description": "Vehicle Fuel",
  "date": "2025-06-21"
}
```

---

### 3. Memory Management

The agent uses conversational memory to maintain context between interactions.

This allows users to continue conversations naturally.

Example:

```text
User: I spent $150 on fuel.
Agent: Expense recorded successfully.

User: Actually make that $175.
Agent: Expense updated successfully.
```

---

### 4. Expense Database Management

Google Sheets serves as the financial database.

The system can:

* Create new expense records
* Read existing expenses
* Update expense entries
* Maintain historical transaction logs

---

### 5. Financial Alerts

When predefined conditions are met, the workflow automatically sends notifications to stakeholders.

Examples:

* High-value expenses
* Unusual spending patterns
* Budget threshold breaches

Notifications are sent through Gmail.

---

### 6. User Confirmation

After processing the request, the agent sends a response back to the user via Telegram.

Example:

```text
Expense successfully recorded.

Category: Fuel
Amount: $150
Date: 21 June 2025
```

---

## Technologies Used

### Automation Platform

* n8n

### Artificial Intelligence

* OpenAI GPT

### Communication Channels

* Telegram
* Gmail

### Data Storage

* Google Sheets

### AI Features

* Natural Language Processing
* Conversational Memory
* Intent Recognition
* Data Extraction

---

## Key Features

### Expense Logging

Users can record expenses through simple messages.

### Expense Retrieval

Users can request previous transactions and spending history.

### Expense Updates

Existing records can be modified through conversation.

### Context Awareness

The AI remembers previous interactions during conversations.

### Automated Alerts

Management receives notifications when important financial events occur.

### Real-Time Responses

Users receive immediate confirmation and feedback.

---

## Business Impact

### Before

* Manual spreadsheet updates
* Repetitive data entry
* Limited financial visibility
* Delayed reporting

### After

* Automated expense recording
* Conversational financial management
* Improved reporting accuracy
* Faster financial tracking
* Reduced administrative workload

---

## Skills Demonstrated

* AI Agent Development
* Workflow Automation
* Conversational AI
* OpenAI Integration
* Process Automation
* Financial Systems Automation
* Google Workspace Integration
* Data Management
* Business Process Optimization
* Systems Design
* Operational Automation

---

## Future Enhancements

Potential improvements include:

* Budget tracking and forecasting
* Expense analytics dashboards
* Multi-user support
* Receipt image processing
* OCR-based expense extraction
* Integration with accounting platforms such as QuickBooks or Xero
* Monthly financial summary reports

---

## Outcome

This project demonstrates how AI agents can be used to automate operational workflows, improve financial record management, and provide a more intuitive user experience through natural language interactions. The solution reduces manual effort while increasing the accuracy and accessibility of financial information.
