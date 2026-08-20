---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 9: Order Is Not Created Using Voice Flow 3

## Problem overview

Your goal is to:

**Investigate why a customer order is not created when the caller completes the order flow with the Autonomous AI Agent.** Use the Webex AI Agent settings, Webex AI Agent Session logs and Voice Flow logs to find the root cause. Do not change the configuration.

---

## Troubleshooting Steps

1. Dial **<copy>+19842990134</copy>** and place an order with the AI agent—for example, say, **This is for birthday party, I need 20 red roses no delivery.**
2. From Control Hub, go to **Contact Center** > **Overview** and open **Webex AI Agent**.
3. Open the AI agent configured for this problem and go to **Actions**.
4. Locate the action used to **create a new order** and review how it is configured.
5. Navigate to **Sessions**, locate the conversation from your test call, and review the session trace for the order creation attempt.
6. Review the related **WxCC voice flow** trace and logs to identify why the order was not created.

## Quiz

??? challenge
