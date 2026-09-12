---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 5: Order Is Not Created Using Webex Connect 3

## Problem overview

After resolving Problem #4, you see the orders are creating properly on the third party application. However, the AI Agent is still responding that the order was not created properly.

Interaction ID: **<copy>5c409ca5-0459-425f-8fe5-090bb242a02f</copy>**

---

## Troubleshooting Steps

1. From the **Webex AI Agent** session logs, find the **Transaction ID** related to the fulfillment. This will help you find the logs in the **Webex Connect** flow for this interaction.
2. Review **Webex Connect** logs for this interaction. Is it still failing?
3. What is the mechanism to return the data from the **Webex Connect** to **Webex AI Agent**?

## Quiz

??? challenge
    <iframe src="https://app.sli.do/event/dCyCXQkNJEmoeVnqKP2Fr5/embed/polls/e5d63edb-fdc6-47e7-87d4-b20c2317f7a1" width="100%" height="400" frameborder="0"></iframe>
