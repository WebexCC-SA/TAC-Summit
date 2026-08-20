---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 2: No Response from the Knowledge Base

## Problem overview

Your goal is to:

**Investigate why the Autonomous AI Agent does not answer questions that should come from the knowledge base.** Use the agent configuration and session logs to find the root cause. Do not change the configuration.

---

## Investigate

### Task 1. Reproduce the issue

1. Sign in to [Webex Control Hub](https://admin.webex.com){:target="_blank"} using one of the lab accounts from the [Lab overview](AI_Lab_Aut_Troubleshoot_Overview.md).
2. Dial **<copy>+19842990134</copy>** and ask a question that should be answered from the knowledge base—for example, ask about available flowers or bouquets.

### Task 2. Review the AI agent and conversation logs

1. From Control Hub, go to **Contact Center** > **Overview** and open **Webex AI Agent**.
2. Open the AI agent configured in the flow for this problem.
3. Review the AI agent configuration and how the **Knowledge Base** is set up for this agent.
4. Navigate to **Sessions**, locate the conversation from your test call, and review the session trace to confirm the knowledge base was not used in the response.
