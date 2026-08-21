---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 1: AI Agent Does Not Answer the Call

## Problem overview

The customer reported that inbound calls are failing as soon as the call reaches the Virtual Agent node. Reproducible all the time. Contact Session ID example of the failed call: **<copy>de302168-d657-4c1c-9cdf-8b159ab6291b</copy>**

---

## Troubleshooting Steps

1. Sign in to [Webex Control Hub](https://admin.webex.com){:target="_blank"} using one of the lab accounts from the [Lab overview](AI_Lab_Aut_Troubleshoot_Overview.md).
2. Find which **flow** is related to the number **<copy>+19842990134</copy>**.
3. Open the flow and search by the **Contact Session ID** the customer provided. You can also try to reproduce the issue and investigate your own example.
4. From the **Trace**, do you see any error? What could be the reason for the error?
5. Find the related **AI Agent** and review the AI Agent configuration. Do you see any issue with misconfiguration or compatibility?

**<details><summary>Hint <span style="color: orange;"></span></summary>**

[Supported languages and voices for AI agents](https://help.webex.com/en-us/article/pdef2d/Supported-languages-and-voices-for-AI-agents){:target="_blank"}

## </details>

## Quiz

??? challenge
    <iframe src="https://app.sli.do/event/qGiGp8xfC2HR2ghtMnh9HB/embed/polls/c65fc190-91f9-4cf0-8acb-812ec271a25b" width="100%" height="400" frameborder="0"></iframe>
