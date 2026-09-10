# n8n Slack Recipe Automation Bot

Recipe Name : Country Chicken Biryani

An automated n8n workflow that listens for recipe requests in Slack, queries an LLM for ingredient lists, formats the output using custom JavaScript, and sends a clean checklist back to Slack.

## 🔄 Workflow Flow
1. **Slack Trigger**: Captures incoming user messages requesting a recipe (tested with *Country Chicken Biryani*).
2. **Edit Fields**: Maps and sets the recipe name variable (`Recipe Name`).
3. **Basic LLM Chain (OpenAI)**: Generates a structured ingredient and quantity list for *Country Chicken Biryani*.
4. **Code in JavaScript**: Cleans text escape sequences (`\n`) to format a proper vertical bulleted list.
5. **Slack (Send Message)**: Delivers the final formatted grocery list back to the channel.

## 📂 Files Included
- `workflow.json`: The complete n8n workflow export.
- `architecture.jpeg`: Screenshot of the canvas workflow nodes.
- `README.md`: Project documentation.
