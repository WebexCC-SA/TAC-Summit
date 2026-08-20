---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 5: MCP Action Does Not Return Order Status

## Problem overview

Your goal is to:

**Investigate why the MCP action does not return the expected order status to the caller.** Use the session logs to find the root cause. Do not change the configuration.

---

## Investigate

### Task 1. Reproduce the issue

1. Sign in to [Webex Control Hub](https://admin.webex.com){:target="_blank"} using one of the lab accounts from the [Lab overview](AI_Lab_Aut_Troubleshoot_Overview.md).
2. Dial **<copy>+19842990134</copy>** and ask for an order status update that should be handled by the MCP action.

### Task 2. Review conversation logs

1. From Control Hub, go to **Contact Center** > **Overview** and open **Webex AI Agent**.
2. Open the AI agent assigned to this problem.
3. Navigate to **Sessions** and locate the conversation from your test call.
4. Review the session trace and identify why the MCP action failed or returned an unexpected result.

### Task 3. Document your finding

1. Write down the root cause you identified from the logs.
2. Be prepared to discuss your finding with the instructor.