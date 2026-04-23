---
#icon: material/folder-open-outline
icon: material/medal
---

# Mission 4: Configure Fulfillment Action and create an order using **Voice Flow**. 

**<details><summary>What is fulfilment Action? <span style="color: orange;"></span></summary>**

Fulfillment Action is a task that an AI agent performs by understanding user intents and completes by connecting to external systems over API. 


## </details>

## Mission overview

Your mission is to:

In the previous Mission you was using Webex Connect flow to execute tha API calls. For this Mission you will be using the Voice flow to execute the API call to create teh order. 

![Profiles](../graphics/Lab1_AI_Agent/Fulfilment.png)

---

## Build

### Task 1. Configure Create_New_Order action to use voice flow for fulfillment.

1. In the AI Agent Studio, open **Create_New_Order** Action.
   ![Profiles](../graphics/Lab1_AI_Agent/19.1.gif)

2. Scroll down and for the **Fulfillment** option select **Manage in the source flow (voice only). Click **Save**
   ![Profiles](../graphics/Lab1_AI_Agent/19.2.png)

### Task 2. Configure fulfillment logic in the Voice flow. 

1. In **Control Hub** got to Flows and open you flow with name **<copy>AutonomousAI_Flow_2000_<w class="attendee"></w></copy>**. Click on **Edit**.
   ![Profiles](../graphics/Lab1_AI_Agent/19.3.gif)

2. Remove **DisconnectContact** node. 
   ![Profiles](../graphics/Lab1_AI_Agent/19.4.gif)

3. Create flow string variable with name **<copy>event_name</copy>** and empty default value.
   ![Profiles](../graphics/Lab1_AI_Agent/19.5.gif) 

4. Create flow string variable with name **<copy>order_request_details</copy>** and empty default value.
   ![Profiles](../graphics/Lab1_AI_Agent/19.6.gif) 

5. Add **SetVariable** node from the left side of flow designer to the field. Connect **VirtualAgentV2** node to the **SetVariable** node. 
   ![Profiles](../graphics/Lab1_AI_Agent/19.7.gif) 

6. Click on the **SetVariable** that you just created and configure your **event_name** variable to be assigned with **VirtualAgentV2....StateEventName** variable. </br>
   **Note:** *This event name will be the same as your Action name from the AI Agent Studio that is used for the fulfillment.*
   ![Profiles](../graphics/Lab1_AI_Agent/19.8.gif)

7. Add one more **SetVariable** node and connect them in series.
   ![Profiles](../graphics/Lab1_AI_Agent/19.9.gif) 

8. We will need to assign the metadata from AI agent to the **order_request_details** string variable. To do so click on **VirtualAgentV2** node, on the right side scroll down until you will see Activity output variable. Copy the name of the variable related to MetaData. Go to your second SetVariable node and configure **order_request_details** with value of the Metadata that you copy inside of the {{}}. See the gif below. 
   ![Profiles](../graphics/Lab1_AI_Agent/19.10.gif) 

9. Add **Case** node and connect **SetVariable** node to the **Case** node.  
   ![Profiles](../graphics/Lab1_AI_Agent/19.11.gif) 

10. Add **Disconnect Contact** and assign the **Default** output on **Case** node to the **Disconnect Contact**
   ![Profiles](../graphics/Lab1_AI_Agent/19.12.gif) 

11. Click on **Case** node. Select **event_name** as the Case Variable. Remove the second Link Description. Keep only one Link Description, as for now you have only one action for fulfillment. In the Link Description provide the name of your action: **<copy>Create_New_Order</copy>**.
   **Note:** *If you add more actions later, the Case node is used as the distribution logic for different fulfillment requests.*
   ![Profiles](../graphics/Lab1_AI_Agent/19.13.gif)

12. Add **HTTP Request** node and connect the **Case** output link to the **HTTP Request** node.
   ![Profiles](../graphics/Lab1_AI_Agent/19.14.gif)

13. Configure the **HTTP Request** with the following:

    - Use authenticated endpoint: **Off**
    - Request URL: **<copy>https://67e9aa0bbdcaa2b7f5b9ed62.mockapi.io/customerOrder</copy>**
    - Method: **POST**
    - Content type: **Application/JSON**
    - Request body: **<copy>{{order_request_details}}</copy>**
       ![Profiles](../graphics/Lab1_AI_Agent/19.15.gif)

14. Connect **HTTP Request** node to **VirtuaAgentV2** node.
   ![Profiles](../graphics/Lab1_AI_Agent/19.16.gif)