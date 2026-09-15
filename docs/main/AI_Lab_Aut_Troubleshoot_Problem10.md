---
#icon: material/folder-open-outline
icon: material/medal
---

# Problem 10: Transfer Call to Wholesale AI Agent Doesn't Have Shared Context

## Problem overview

The customer is testing **Webex AI Agent** to **Webex AI Agent** transfer but complains that the second AI agent doesn't have the context that was already discussed between the caller and the first AI agent. This is a bad experience as the caller has to repeat themselves. Interaction ID **<copy>51b2459e-05b7-40d6-b117-14a372e5d1a0</copy>**.

---

## Troubleshooting Steps

1. Investigate the **AI Agent Session** logs for Webex AI Agents **<copy>180_2000_AutoAI_Lab</copy>** and **Flower_Wholesale**.
2. Investigate the **Voice Flow** design to understand why the context was not sent from one AI agent to another AI agent.

**<details><summary>Hint <span style="color: orange;"></span></summary>**

[Multi-agent orchestration](https://help.webex.com/en-us/article/5a07xcb/Multi-agent-orchestration){:target="_blank"}

## </details>

## Quiz

??? challenge
    <iframe src="https://app.sli.do/event/vAGJVH9TGfQGLExv4VYijU/embed/polls/d4907a09-dbf5-45f1-a5e6-f3e9b91775f0" width="100%" height="400" frameborder="0"></iframe>
