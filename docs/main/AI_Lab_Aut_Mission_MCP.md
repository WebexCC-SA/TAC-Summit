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

For this mission, the MCP server was created and deployed on AWS with two tools:</br>
1) Check Flower Store Locations. </br>
2) Check the order status by sending API call with the order ID to the MockAPI repository. </br>

This MCP Sever repository you can find on github below. In the **READMe.md** file you will be able to fine instructions on how ot deploy it on AWS. You can use it as the example for implementing the MCP server for you production tenant, but for this lab it is already deployed so the link below is just the reference of the source code. </br>
</br>
**<copy>https://github.com/mdanylch/store_address_2000</copy>**

**In this mission you will work on adding this External MCP server to Webex cloud and plug it in with you AI Agent.**

![Profiles](../graphics/Lab1_AI_Agent/MCPAction.png)

---

## Build

### Task 1. Create Agentic App in Webex Developer Portal. 

1. Open [Webex Developer Portal](https://developer.webex.com/){:target="_blank"} .

2. Click on **Login**. Login with you admin credentials.
![Profiles](../graphics/Lab1_AI_Agent/15.1.png)

3. Under the Profile, click on **My Webex App**
![Profiles](../graphics/Lab1_AI_Agent/15.2.png)

4. Click on **Create a New App**.
![Profiles](../graphics/Lab1_AI_Agent/15.3.png)

5. On the next page, select **Create an Agentic App**.
![Profiles](../graphics/Lab1_AI_Agent/15.4.png)

6. Name you app as **<copy><w class="attendee"></w>\_MCP_Server</copy>**
![Profiles](../graphics/Lab1_AI_Agent/15.5.png)

7. For **Agent App Description**, paste the text below (use the **copy** icon on the code block):

    ``` text
    This MCP server is used for the following:

    1) Check the flower store locations
    2) Check the order status based on the order ID.
    ```
![Profiles](../graphics/Lab1_AI_Agent/15.6.png)

8. Select an available Agentic App Icon. Click 2 times on an Icon. 
![Profiles](../graphics/Lab1_AI_Agent/15.7.gif)

9. For the Agentic App URL enter **<copy>https://y4drgmvgpb.us-east-1.awsapprunner.com/mcp</copy>** and for Agentic App auth type select **Custom Headers**. Finally click on **Add Agentic App**.
![Profiles](../graphics/Lab1_AI_Agent/15.7.gif)










<p style="text-align:center"><strong>Congratulations, you have officially completed this mission! 🎉🎉 </strong></p>
