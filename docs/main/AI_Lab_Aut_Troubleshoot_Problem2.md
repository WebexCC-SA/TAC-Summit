---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 2: Order Is Not Created Using Webex Connect

## Problem overview

We just created the new Action that should create a new order with our third party system. However, the AI agent responds that the order cannot be completed for some reason. Contact Session ID: **<copy>e7b000c9-780f-4619-91c5-51ee1dbecb19</copy>**

---

## Troubleshooting Steps

1. Investigate the **Contact Session ID** in the voice flow. Do you see any problems?
2. Investigate the **Contact Session ID** in the **Webex AI Agent** **Sessions**. Was the **Create_New_Order** action executed?
3. Review the configuration of the **Create_New_Order** action. What kind of fulfillment is configured, and what flow is used in this action?
4. Review the **Connect Flow** configuration.

**<details><summary>Hint <span style="color: orange;"></span></summary>**

In the **AI Agent Session Details** report, check what **Webex Connect Flow** is configured for the fulfillment and how the flow is configured.

## </details>

## Quiz

??? challenge
    <iframe src="https://app.sli.do/event/qDCfRaWTiechgKoHU42QsP/embed/polls/53f72481-48b2-406c-8f4e-dd7f3e3a3b32" width="100%" height="400" frameborder="0"></iframe>