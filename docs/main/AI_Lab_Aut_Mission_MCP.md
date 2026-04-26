---
#icon: material/folder-open-outline
icon: material/medal
---

# Mission 7: Configure Action with MCP

**<details><summary>What is MCP? <span style="color: orange;"></span></summary>**

MCP, or Model Context Protocol, is a standardized framework designed to facilitate the exchange of contextual information between AI models and external systems, enabling more dynamic and context-aware interactions. By using MCP, AI agents can be easily integrated with other external tools, allowing for different types of fulfillment.

## </details>

## Mission overview

In Mission 3, you configured fulfillment by adding an HTTP request node to your voice flow to create an order. Imagine that this HTTP request could be preconfigured on a server, and you simply need to connect your AI agent to that server to utilize it.</br>
</br>
Using an MCP (Model Context Protocol) server is a highly practical approach. If you manage multiple agents and need to configure various fulfillment options for them, you no longer need to rebuild the same logic repeatedly within your flows. Instead, you can simply connect an MCP server and select the specific tool you need. You will love it!</br>

For this mission, the MCP server was created with two tools:</br>
1) Check Flower Store Locations. </br>
2) Check the order status by sending API call with the order ID to the MockAPI repository. </br>

This MCP Sever repository you can find on github below. In the **READMe.md** file you will be able to fine instructions on how ot deploy it on AWS. You can use it as the example for implementing the MCP server for you production tenant.</br>
https://github.com/mdanylch/store_address_2000

![Profiles](../graphics/Lab1_AI_Agent/MCPAction.png)

---

## Build

### Task 1. Create MCP Action

1. Open up your AI Agent **<copy><w class="attendee"></w>\_2000_AutoAI_Lab</copy>** and start creating the new **Action**.
   ![Profiles](../graphics/Lab1_AI_Agent/15.1.gif)

2. From the list, select **get_store_locations** MCP option.
   ![Profiles](../graphics/Lab1_AI_Agent/15.2.png)

3. You can see that another Action was created, and some of the configurations, such as Description and Entity, were transferred from the MCP server. This new Action essentially adds functionality to the AI Agent, enabling it to provide customers with store locations. These location details are stored in a third-party database and are accessed through the MCP integration.
   ![Profiles](../graphics/Lab1_AI_Agent/15.3.png)

4. **Publish** the changes.
   ![Profiles](../graphics/Lab1_AI_Agent/15.4.png)

### Task 2. Test MCP Action

1. You can test the functionality using the chat **Preview** option. Ask the AI agent **<copy>What are the store locations?</copy>**. The information that the AI agent will respond with will be retrieved from the external database over the MCP.
   ![Profiles](../graphics/Lab1_AI_Agent/15.5.png)

2. Open up the interaction transcripts in the **Session** tab to confirm that result came from the MCP tool.
   ![Profiles](../graphics/Lab1_AI_Agent/15.6.gif)

<p style="text-align:center"><strong>Congratulations, you have officially completed this mission! 🎉🎉 </strong></p>
