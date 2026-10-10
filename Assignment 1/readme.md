Project Overview

This project focuses on building an automated payment follow-up system by integrating Zapier with Google Sheets and Gmail.

The workflow checks invoice details stored in a spreadsheet, detects records with outstanding payments, and sends customized reminder emails to predefined test recipients. Once an email is sent, the corresponding spreadsheet entry is updated to maintain a record of the reminder activity.

Objective

The primary goal is to simplify payment follow-ups by automating the process of tracking unpaid invoices and notifying recipients through email.

The system demonstrates the implementation of the following features:

Scheduled Execution: Runs the automation at predefined intervals.

Spreadsheet Integration: Retrieves invoice and payment information from Google Sheets.

Conditional Filtering: Selects records where the payment status is pending.

Data Validation: Checks whether an email address is available before proceeding.

Automated Email Notifications: Sends personalized payment reminder messages through Gmail.

Record Management: Updates the relevant spreadsheet row after the reminder is sent.

Reminder Status Tracking: Maintains a record of completed reminder actions.

Tools and Technologies

Zapier – Workflow automation and application integration

Google Sheets – Invoice data storage and payment status management

Gmail – Automated email delivery

Google Drive – File storage and management

CSV / Excel – Spreadsheet data preparation and import

Workflow

Schedule by Zapier
        ↓
Google Sheets – Retrieve Multiple Rows
        ↓
Filter – Identify Pending Payments
        ↓
Filter – Verify Email Availability
        ↓
Gmail – Send Personalized Payment Reminder
        ↓
Google Sheets – Update Reminder Status

Expected Outcome

The completed workflow reduces manual effort in monitoring unpaid invoices and sending follow-up emails. It also improves consistency in payment reminders and provides a simple tracking mechanism for recording reminder activity in the spreadsheet.
