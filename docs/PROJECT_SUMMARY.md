# Private School AI Enrollment Lead Qualification

## Purpose
This project is built to help Myanmar private schools automatically review and prioritize student enrollment inquiries.

Its purpose is to reduce manual admission workload, respond faster to serious parent inquiries, and help school staff focus first on the most valuable and urgent leads.

## Problem
Private schools often collect enrollment inquiries through online forms, but admission teams usually need to review every submission manually.

This creates several business problems:

- Slow response time to parents
- Manual and repetitive lead checking
- Difficulty identifying high-intent inquiries
- Inconsistent prioritization between leads
- Duplicate submissions causing confusion
- More admin work for admission staff

Because of this, schools may miss strong enrollment opportunities or spend too much time on low-priority inquiries.

## Solution
This project automates the first stage of student enrollment lead qualification.

The workflow collects form submissions, validates the data, checks for duplicate inquiries, and uses AI to analyze the parent’s message and enrollment intent.

Then it:

- assigns a lead score
- classifies the inquiry as HOT, WARM, or COLD
- recommends the next action
- stores the result in Google Sheets
- sends Telegram alerts for important leads
- handles workflow or AI errors through a separate error workflow

This helps the school admission team work faster, stay organized, and follow up with the right parents at the right time.

## Tools Used
- **n8n** — workflow automation
- **Google Forms** — lead collection form
- **Google Sheets** — lead database and tracking
- **Google Gemini API** — AI lead qualification
- **Telegram Bot** — HOT lead notifications
- **Telegram Channel / Group** — admin alerts and updates

## Workflow Summary
1. Parent submits the enrollment form  
2. n8n receives the new form response  
3. The workflow validates required fields  
4. It checks whether the inquiry is a duplicate  
5. If needed, AI analyzes the lead  
6. The system generates score, priority, and recommendation  
7. Results are saved to Google Sheets  
8. HOT leads are sent to Telegram  
9. Errors are handled by the separate error workflow

## Business Value
This system helps private schools:

- reduce manual admission work
- improve response speed
- identify high-intent parents quickly
- keep lead records organized
- minimize duplicate processing
- create a more professional enrollment pipeline