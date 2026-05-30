---
#icon: material/folder-open-outline
icon: material/medal
---

# Mission 1: Create AI Autonomous Agent

## Mission overview

Your mission is to:

**Create an AI agent and upload the knowledge base (KB)** to enable the agent to provide answers about available flowers and assist customers with creating an order or transferring the interaction to a human agent.
![Profiles](<../graphics/Lab1_AI_Agent/Untitled(9).jpg>)

---

## Build

### Task 1. Create a new AI Agent with Knowladge Base

1. Download the .xlsx file [Flowrs_Catalog](https://docs.google.com/spreadsheets/d/1A5d1ZEPWmPE_38Bi8bVULKLhCH0wyGX4/edit?usp=sharing&ouid=100862210011127627593&rtpof=true&sd=true){:target="\_blank"}.
   > **Flower_Catalog.xlsx** - file contains information on the available single flowers and bouquets, including the price of the flowers or bouquets and occasions that suit the flowers.
   ![Profiles](../graphics/Lab1_AI_Agent/2.74.png)
2. Microsoft office is not installed on this PC so you cannot open the file directly to review it. So please review the screenshots below to understand the file content that you will be using for you Knowledge base.
   ![Profiles](../graphics/Lab1_AI_Agent/Knowledge1.png)
   ![Profiles](../graphics/Lab1_AI_Agent/Knowledge2.png)
   ![Profiles](../graphics/Lab1_AI_Agent/Knowledge3.png)

3. Go to [Webex Control Hub](https://admin.webex.com){:target="\_blank"}.

4. Open **Contact Center** from the left side navigation panel, and under **Overview > Quick Links**, click on **Webex AI Agent**.
   ![Profiles](../graphics/Lab1_AI_Agent/L1M6_OpenWebexAI1.gif)



5. In AI Agent Builder, navigate to **Knowledge** from the menu panel on the left side.

6. Click **Create Knowledge Base**, provide Knowledge base name as **<copy><w class="attendee"></w>\_2000_AI_KB</copy>**, then click **Create**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.1.gif)

7. Click on **Upload Files**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.1.a.png)

8. Click **Add File** or drag and drop the downloaded file **Flower_Catalog.xlsx** you downloaded on **Step 1**. Then click **Process Files**. Wait until the file is processed. 
   ![Profiles](../graphics/Lab1_AI_Agent/2.2.gif)


9. <span style="color: red;">[Read Only]</span> : You can also create an Article or refer your Websites for the Knowledge source. 
   ![Profiles](../graphics/Lab1_AI_Agent/2.2.a.png)

10. Navigate to **AI Agents** from the left-hand side menu panel and click on **Create Agent**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.58.gif)
11. Select **Start from Scratch** and click **Next**.
12. On **Create an AI agent** page select the following select the type of agent: **Autonomous**.

13. Provide the following information in the **Add the essential details**, then click **Create**:

    > Agent Name: **<copy><w class="attendee"></w>\_2000_AutoAI_Lab</copy>**
    >
    > System ID is created automatically
    >
    > AI engine: **Webex AI Pro 1.0**
    >
    > Agent's goal: **_<copy>This is Flower Shop. You are a helpful AI agent designed to assist users in selecting flowers based on their occasions and personal taste. You can also set up delivery and send a confirmation SMS with the order details. Do the math for the total flower price. For example if the agent want to order 20 roses and the price for one rose is 20 $ in the knowledge base it should calculate the total as 400 $. Add delivery 50 to the total if require.</copy>_**

    > <span style="color: red;">[Read Only]</span> Here you can find the best practices on how to write the  Agent"s goal.
    >  [Do's and Don'ts when writing goals](https://help.webex.com/en-us/article/nelkmxk/Guidelines-and-best-practices-for-automating-with-AI-agent#concept-template_96114022-037a-46be-80ce-bf8c6b0d67c0){:target="_blank"}


    ![Profiles](../graphics/Lab1_AI_Agent/2.3.gif)

14. Customize the Welcome message with: **_<copy>Hi there, my name is Blossom, the AI Agent. How can I assist you?</copy>_**

    ![Profiles](../graphics/Lab1_AI_Agent/2.16.png)

15. In the instructions, add additional specific guidelines that you would like the AI Agent to follow. Just **copy the text below and paste it to the Instructions section** (use the **copy** icon on the code block): <br>

    ``` text
    If the customer wants to order any number of boxes of roses transfer it to Wholesale department. Use the Action Transfer_to_different_department to transfer the call.

    Use the knowledge base to:
    - check the flower catalog
    - provide relevant recommendations
    - confirm availability and pricing
    - calculate the full order total based on selected items and delivery

    Core Behavior

    Start by asking for the occasion or purpose of the flowers.
    Recommend flowers or bouquets based on:
    - occasion
    - customer preferences
    - budget
    Use the knowledge base to provide:
    - flower descriptions
    - prices
    - meanings
    - seasonal availability
    Help the customer customize the bouquet if needed.
    If delivery is requested:
    - collect the address
    - repeat it back for confirmation
    - add delivery cost to the total
    Before completing the order:
    - show a clear order summary
    - confirm the final total
    - ask if the customer wants SMS confirmation

    Communication Style

    Be friendly, clear, and concise.
    Keep the conversation focused on flower shopping.
    If something is unclear, ask a simple follow-up question.
    Maintain context from earlier messages.

    Guardrails

    Do not guess catalog items, prices, or availability.
    Always rely on the knowledge base for product and pricing information.
    Avoid unrelated or off-topic conversations.
    ```

    ![Profiles](../graphics/Lab1_AI_Agent/2.4.png)

16. <span style="color: red;">[Read Only]</span> Here you can find the best practices on how to write the  Instructions: [Prompt engineering tips when writing instructions](https://help.webex.com/en-us/article/nelkmxk/Guidelines-and-best-practices-for-automating-with-AI-agent#concept-template_96114022-037a-46be-80ce-bf8c6b0d67c0){:target="_blank"}

17. Switch to **Knowledge** tab. From drop-down list, search for **<copy><w class="attendee"></w>\_2000_AI_KB</copy>**. If you don't see your **Knowledge base** in the list it still could be processing. Then select the one we processed earlier for your user. From **Knowledge base** drop-down list, select **<copy><w class="attendee"></w>\_2000_AI_KB_Plan_B</copy>**. Click on **Save changes**.
    ![Profiles](../graphics/Lab1_AI_Agent/2.5.gif)

18. **Publish** the AI Agent. Provide any version name in popped up window (e.g. "V1").<br>
    ![Profiles](../graphics/Lab1_AI_Agent/2.6.gif)

### Task 2. Test your AI Agent

1. Click on **Preview** and test the AI Agent to understand how it behaves using the **chat channel** by clicking on **Start a chat**. You can start the conversation with: **<copy>I need flower for my friend</copy>**. And try to ask what is the flower availability and prices and what would be the total for some flower that you select.
   ![Profiles](../graphics/Lab1_AI_Agent/2.59.gif)

2. Click on **Preview** and test the AI Agent to understand how it behaves using the **voice channel** by clicking on **Start a call**. You can start the conversation with: **"I need flower for my friend"**<span class="copy-static" title="Click to copy!" data-copy-text="I need flowers for my friend"><span class="copy"></span></span> and try to customize your order.
   > **Note:** This Lab is being conducted in a classroom with approximately 20 attendees.  
   > Environmental factors, such as background noise and other attendees speaking next to you, may affect the response accuracy.  
   > For best results, it is **strongly recommended to use computer headphones**, if available.

![Profiles](../graphics/Lab1_AI_Agent/2.60.gif)

<p style="text-align:center"><strong>Congratulations, you have officially completed this mission! 🎉🎉 </strong></p>
