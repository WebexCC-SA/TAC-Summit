---
#icon: material/folder-open-outline
icon: material/medal
---

# Mission 2: Integrating the AI Agent with Flow for Voice Calls

## Mission overview

Your mission is to:

Integrate the AI Agent with the Voice Flow.

### Task 1. Build WxCC voice flow with AI Agent.

1. Open [Control Hub](https://admin.webex.com){:target="_blank"} and go to **Contact Center** navigate to **Flows**, click on **Manage Flows** dropdown list and select **Create Flows**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.47.gif)

2. One the next page select **Start from scratch** and click on **Next**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.48.a.png)

3. Name the new flow **<copy>AutonomousAI_Flow_2000_<w class="attendee"></w></copy>** and click on **Create Flow**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.48.png)

4. Make sure the **Edit** mode at the top is set to **ON**. Then, drag and drop the **Virtual Agent V2** and **Disconnect Contact** activities from the left panel onto the Design field.
    ![Profiles](../graphics/Lab1_AI_Agent/2.49.a.gif)

5. Connect the nodes and configure **VirtualAgentV2**:

    - Connect the **New Phone Contact** output node edge to this **VirtualAgentV2** node.
    - Connect the **Handled** outputs to **DisconnectContact**.
    - Click on the **VirtualAgentV2** block and select **Static Contact Center AI Config**.
    - Select Contact Center AI Config as **Webex AI Agent (Autonomous)**.
    - Virtual Agent: **<copy><w class="attendee"></w>\_2000_AutoAI_Lab</copy>**

    ![Profiles](../graphics/Lab1_AI_Agent/2.49.gif)

6. Drag and drop **Queue Contact** and **Play Music** nodes. Configure them as the following:

    - **Queue Contact**
    - Connect the **Escalated** path from the **Virtual Agent V2** activity to the **Queue Contact** activity.
    - Connect the **Queue Contact** activity to the **Play Music** activity.
    - Click on the **Queue Contact** node and select **Static Queue**.
    - Queue name: **TS_Voice_Queue**
    - **Play Music**
    - Create a loop by connecting the Play Music activity back to itself - to create a music loop, following the example provided below.
    - Click on the **Play Music** node and select Music File: **defaultmusic_on_hold.wav**.

    ![Profiles](../graphics/Lab1_AI_Agent/2.50.gif)

7. **Validate** and **Publish** Flow. In the popped up window, click on dropdown menu to select **Latest** label (**DO NOT** Select any other tag but only **Latest**), then click **Publish**.
   ![Profiles](../graphics/Lab1_AI_Agent/2.51.gif)

8. Go to **Channels**, find the channel with name **180_2000_Channel** and make the copy of it. 
   ![Profiles](../graphics/Lab1_AI_Agent/2.52a.png)

9. Rename the Channel by replacing the **180** with your **last name**1 and removing everything after Channel.
   ![Profiles](../graphics/Lab1_AI_Agent/2.52e.png) 

10. Select the routing flow that you have created earlier.
   ![Profiles](../graphics/Lab1_AI_Agent/2.52d.png)


11. On the buttom select any number from Site1 pool.
   ![Profiles](../graphics/Lab1_AI_Agent/2.52b.png)

12. Click on **Create**
  ![Profiles](../graphics/Lab1_AI_Agent/2.52c.png)


13. Dial the support number assigned to your **<w class="attendee"></w>\_2000_Channel** to test the Autonomous AI Agent over a voice call.
   ![Profiles](../graphics/Lab1_AI_Agent/2.84.png)

<p style="text-align:center"><strong>Congratulations, you have officially completed the Autonomous AI Agent lab! 🎉🎉 </strong></p>
