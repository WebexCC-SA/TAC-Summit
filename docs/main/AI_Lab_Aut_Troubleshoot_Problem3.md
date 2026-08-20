---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 3: Order Is Not Created Using Webex Connect

## Problem overview

Your goal is to:

**Investigate why a customer order is not created when the caller completes the order flow with the Autonomous AI Agent.** Use the agent configuration, action settings, and session logs to find the root cause. Do not change the configuration.

---

## Investigate

### Task 1. Reproduce the issue

1. Sign in to [Webex Control Hub](https://admin.webex.com){:target="_blank"} using one of the lab accounts from the [Lab overview](AI_Lab_Aut_Troubleshoot_Overview.md).
2. Dial **<copy>+19842990134</copy>** and place an order with the AI agent—for example, say, **This is for birthday party, I need 20 red roses no delivery.**
3. Note whether the agent confirms the order and provides an order ID.

### Task 2. Review the action and conversation logs

1. From Control Hub, go to **Contact Center** > **Overview** and open **Webex AI Agent**.
2. Open the AI agent configured for this problem and go to **Actions**.
3. Locate the action used to **create a new order** and review how it is configured.
4. Navigate to **Sessions**, locate the conversation from your test call, and review the session trace for the order creation attempt.
5. From the trace, follow what happens when the action runs. What flow does the action call? Review that flow configuration and identify why the order was not created.
