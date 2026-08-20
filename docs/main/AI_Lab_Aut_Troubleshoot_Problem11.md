---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 11: Transfer Call to Wholesale AI Agent Doesn't Have Shared Context

## Problem overview

Your goal is to:

**Investigate why shared context is not passed when the call is transferred to the Wholesale AI Agent.** Use the Webex AI Agent settings, session logs, and voice flow trace to find the root cause. Do not change the configuration.

---

## Troubleshooting Steps

1. Dial **<copy>+19842990134</copy>** and ask to be transferred to the **Wholesale** department.
2. From Control Hub, go to **Contact Center** > **Overview** and open **Webex AI Agent**.
3. Open the AI agent configured for this problem and go to **Actions**.
4. Locate the **transfer** action used for the Wholesale department and review how it is configured.
5. Navigate to **Sessions**, locate the conversation from your test call, and review the session trace for the transfer attempt.
6. Review the related **WxCC voice flow** trace and the **Wholesale AI Agent** session to identify why shared context was not available after the transfer.

## Quiz

??? challenge
