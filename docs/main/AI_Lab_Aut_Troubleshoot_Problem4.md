---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 4: Transfer to Queue Fails

## Problem overview

Your goal is to:

**Investigate why the transfer action does not route the caller to the correct queue.** Use the session logs to find the root cause. Do not change the configuration.

---

## Investigate

### Task 1. Reproduce the issue

1. Sign in to [Webex Control Hub](https://admin.webex.com){:target="_blank"} using one of the lab accounts from the [Lab overview](AI_Lab_Aut_Troubleshoot_Overview.md).
2. Dial **<copy>+19842990134</copy>** and request a transfer to the department described by your instructor.

### Task 2. Review conversation logs

1. From Control Hub, go to **Contact Center** > **Overview** and open **Webex AI Agent**.
2. Open the AI agent assigned to this problem.
3. Navigate to **Sessions** and locate the conversation from your test call.
4. Review the session trace and identify why the transfer action failed or routed incorrectly.

### Task 3. Document your finding

1. Write down the root cause you identified from the logs.
2. Be prepared to discuss your finding with the instructor.