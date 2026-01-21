# n8n Workflow Explanation

1. Trigger
- Gmail trigger checks for new incoming emails

2. Data Extraction
- Email subject and body are extracted

3. AI Classification
- Email content is sent to the LLM
- Classified into: Job, Support, Sales, Spam, Other

4. Decision Logic
- IF node routes emails based on category

5. Auto-Response
- Predefined response is sent for Support/Sales
- Job emails are logged only

6. Logging
- Email metadata is stored in Google Sheets
