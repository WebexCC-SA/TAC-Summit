---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 10: Transfer Call to HR Queue Landed on the Default Queue

## Problem overview

Your goal is to:

**Investigate why a caller who requests a transfer to the HR queue is routed to the default queue instead.** Use the Webex AI Agent settings, session logs, and voice flow trace to find the root cause. Do not change the configuration.

---

## Troubleshooting Steps

1. Dial **<copy>+19842990134</copy>** and ask to be transferred to the **HR** department.
2. From Control Hub, go to **Contact Center** > **Overview** and open **Webex AI Agent**.
3. Open the AI agent configured for this problem and go to **Actions**.
4. Locate the **transfer** action and review how it is configured.
5. Navigate to **Sessions**, locate the conversation from your test call, and review the session trace for the transfer attempt.
6. Review the related **WxCC voice flow** trace and identify why the call was routed to the default queue instead of the HR queue.

## Quiz

??? challenge
