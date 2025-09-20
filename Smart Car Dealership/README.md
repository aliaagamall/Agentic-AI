### Smart Car Dealership Automation Workflow

#### Description
The **Smart Car Dealership Automation Workflow** is an automation project built using n8n. It automates the process of notifying the dealership owner via email and logging sale details in a Google Sheet whenever a car is sold. This reduces manual work, minimizes errors, and ensures real-time updates for the owner.

#### Features
- **Webhook Trigger**: Captures car sale data (car type, price, buyer) via a POST request from the dealership’s system.
- **Email Notification**: Sends an email to the owner with sale details (e.g., "A Car has just been sold: [Toyota Camry, $24,000, Sarah Johnson]").
- **Google Sheets Integration**: Appends sale data to a Google Sheet for record-keeping.
- **Efficiency**: Automates data handling to prevent errors and save time.

#### Technologies
- **n8n**: Workflow automation platform.
- **Webhook**: Handles incoming POST requests with sale data.
- **Gmail API**: Sends automated email notifications.
- **Google Sheets API**: Logs data in a spreadsheet.
- **Postman**: Used for testing the webhook.

#### Setup
1. Install and set up n8n locally or on a self-hosted server.
2. Import the `Smart Car Dealership Workflow.json` file into n8n.
3. Configure OAuth2 credentials for Gmail and Google Sheets in n8n.
4. Create a Google Sheet with columns `Car`, `Price`, and `Buyer`, and update the `documentId` in the JSON.
5. Test the workflow using Postman with a JSON payload (e.g., `{ "Car": "Toyota Camry", "Price": 24000, "Buyer": "Sarah Johnson" }`).
6. Activate the workflow in n8n for live use.

#### Sample JSON Payload
```json
{
  "Car": "Toyota Camry",
  "Price": 24000,
  "Buyer": "Sarah Johnson"
}
```





