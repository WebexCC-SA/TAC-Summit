---
#icon: material/folder-open-outline
icon: material/bullseye-arrow
---

<!-- Markdown content with embedded HTML -->
<div>
    <h3><b>Please submit the Attendee as your last name.</b></h3> 
    <h3>All configuration entries in the lab guide will be renamed to include your Attendee ID.</h3>
    <form id="info">
        <label for="attendee">Attendee ID:</label>
        <input type="text" id="attendee" name="attendee" placeholder="Enter your last name" required>
        <button onclick="setValues()">Save</button>
    </form>

    <br>

    <p>Your stored Attendee ID is:<w class="attendee"> No ID stored</w></p>

</div>

## Overview of the lab's Use Case


You are designing a **Webex AI Agent** for a flower shop to assist customers with answering questions and ordering flowers. To support agents and supervisors with the latest AI tools, you will configure **AI Assistant** features.

[Webex AI Agent use case example](https://blog.webex.com/customer-experience/announcing-general-availability-of-webex-ai-agent-paving-way-new-era-cx/){:target="_blank"}

### AI Agent Capabilities

- **Recommending flowers based on customer preferences or occasions**
- **Collecting order details for both standard and custom bouquets**
- **Calculating total price in real time**
- **Gathering delivery information, including address and delivery date**
- **Provide the order status using the integration with MCP server**
- **Transferring to a specific queue with human agents, when needed for complex inquiries**

## Disclaimer

The lab design and configuration examples provided are for educational purposes. For production design queries, please consult your Cisco representative or an authorized Cisco partner.
Let’s get started and discover how **Webex Contact Center Flow Designer** takes customer experiences from good to great!
