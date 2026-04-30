Here's your Incident Communication Command Center — a full 3-column executive briefing tool.

What's inside, mapped to your wireframes:
Left panel mirrors your Image 1 workflow — CGX service info (Apps, App SVC ID, SRE Contact, Business Contact), dependent services (SDR/EPSS/Demographics with live status badges), and the 5-step workflow from "Enter Service Info" → "Distribute to Stakeholders."
Center panel is the comms engine:

5 channel tabs — Teams (Executives, IT, Business) and Outlook (End of Day Summary, Prior Day Report) — matching your Image 2 distribution tree exactly
Each tab renders a pre-drafted, role-appropriate message pulled from ServiceNow + Databricks context
Send marks stakeholders as notified; Regenerate re-loads the draft
Live incident timeline and a ServiceNow SQL query snippet showing the background data fetch

The right panel shows Databricks impact metrics (error rate, affected users, pipeline health), stakeholder notification status, and the Azure Portal vendor reference from your diagram.

Teams source banner — sits above the incident list in the left panel, showing the #cgx-incidents channel as the source with a last-sync timestamp. Hit ↻ Sync to simulate a live pull (timestamp updates to "just now").
"View Details ▾" button on each incident card — clicking it opens an inline drawer directly below that card. A spinner briefly simulates the background fetch from ServiceNow/Databricks before data appears.
Two tabs inside each drawer:

ServiceNow — ticket metadata: priority, state, opened time, assigned team, affected CI, root cause
Databricks — live metrics with mini bar charts: error rate, availability %, affected users, pipeline job status, API 5xx rate, etc.

Each incident has its own independent drawer with its own data, and switching tabs re-triggers the loading animation to simulate a fresh API call.
