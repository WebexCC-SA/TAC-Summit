---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 4: Order Is Not Created Using Webex Connect 2

## Problem overview

After you resolve Problem #3, the customer responded:

It is still not working! Could you please check what is the problem?

Interaction ID: **<copy>9cd6feb8-dc17-450b-b68c-2561705b3b3c</copy>**

I can create a test order using Postman with the following:

**POST**

**<copy>https://67e9aa0bbdcaa2b7f5b9ed62.mockapi.io/customerOrder</copy>**

**Body**

```json
{
    "orderDetails": "Romantic Roses standard bouquet",
    "orderTotal": "100 dollars",
    "delivery": "",
    "address": "north 24 corner zimbave",
    "status": "new",
    "id": "4",
    "phoneNumber": ""
}
```

---

## Troubleshooting Steps

1. Investigate the **Contact Session ID** in the **Webex AI Agent** **Sessions**. Was the **Create_New_Order** action executed?
2. Review the configuration of the **Create_New_Order** action. What kind of fulfillment is configured, and what flow is used in this action?
3. Review the **Connect Flow** configuration.
4. From the **Webex AI Agent** session logs, find the **Transaction ID** related to the fulfillment. This will help you find the logs in the **Webex Connect** flow for this interaction.
5. Review **Webex Connect** logs for this interaction. Where is the call failing?

## Quiz

??? challenge
    <iframe src="https://app.sli.do/event/jvi3jHZxV6JqWeyNZrqAqE/embed/polls/41263d5d-6d91-4c76-aba8-708a597e8f9f" width="100%" height="400" frameborder="0"></iframe>
