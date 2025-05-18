<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- [Intake](https://github.com/MatthewThompsonIT/ticket-lifecycle/edit/main/README.md#intake)
- [Assignment and Communication]()
- [Working the Issue]()
- [Resolution]()

<h2>Intake</h2>

>[!NOTE]
> The Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php 
> End Users osTicket URL: http://localhost/osTicket


- Log in as an End User (End Users osTicket URL: http://localhost/osTicket)
- Click on "Open a New Ticket"

![image](https://github.com/user-attachments/assets/76bc386f-f733-4bed-b70e-07cda8ecfaef)

- Fill out the Contact Information with whatever you made Karen or Ken's information
- Pick "Report a Problem" for the Help Topic (We are going to simulate the entire mobile/online banking system is down)

![image](https://github.com/user-attachments/assets/3f5d1cbe-b89d-4e4f-87b1-39d7a5e0cfa1)

>[!NOTE]
> This would be considered a "Report a Problem/ Critical Outage" but end users dont always put the correct Help Topic so we will simulate fixing that

- Fill out the Ticket Details
- For Issue Summary put: "Entire mobile/online banking system is down"
- For The Description: "My Employees are reporting that users are no longer able to access the online banking portal. The ones who can ocasionally access it, cannot log in."
- Hit "Create Ticket"

![image](https://github.com/user-attachments/assets/e4b69301-460b-4d61-af5a-b3bf36c995e1)

<h2>Assignment and Communication</h2>

- Now lets sign into the Admin Panel as John (http://localhost/osTicket/scp/login.php)
- There will be the ticket that we just created
- Click on the ticket

![image](https://github.com/user-attachments/assets/f9f1813d-498d-49fa-b839-920e686541df)

- Observe the ticket as John and check to see if anything needs to be changed

![image](https://github.com/user-attachments/assets/32b29e99-9a5c-4ab8-9aca-c33cf9231708)

>[!NOTE]
> It is best to contact the creator of the ticket as soon as possible to talk to them and get a better understanding of the ticket.

- We can see that the Priority is set to "Normal"
- The Ticket is "Unassigned"
- The SLA Plan is "Default SLA"
- The Help Topic is "Report a Problem"
- All of this needs to be changed as it does not match the urgency of the ticket
- We want to change the ticket properties to:
  - Priority: "Emergency"
  - SLA Plan: Sev-A (1 hour, 24/7)
  - Assigned To: Online Banking Department
  - Help Topic: "Report a Problem/ Business Critical Outage"
- Click on the "SLA Plan:"
- Change the SLA to: "SEV-A" as this is an urgent problem
- For the description write: "Wide impact, customers are unable to do online banking."

![image](https://github.com/user-attachments/assets/5a4f6d32-d66f-422e-a4c1-8a8d2000f5e8)

- Click on "Help Topic"
- Change it to "Report a Problem/ Business Critical Outage"
- For the description write: "No customers are able to access Online Banking."

![image](https://github.com/user-attachments/assets/214e628d-0e60-445b-bd18-50a7187af32f)

- Click on "Assigned To:"
- Change the Assignee to "Online Banking"
- For the description write: Customers are unable to access the Online Banking portal. Assinging to the Online Banking Team.

![image](https://github.com/user-attachments/assets/ce4fa9b8-17cc-49a3-b595-9c7a387ab4fd)

- Click on "Priority"
- Change the Priority Level to "Emergency"

![image](https://github.com/user-attachments/assets/9d7eb967-6029-4009-ab54-6bd50e93deda)

<h2>Working the Issue</h2>

- Now lets work the ticket to completion as Jane
- Log out of the John account
- Sign into Jane
- Click on the ticket
- Lets assign the ticket to ourself
  - Click on Assigned To: and change it to Jane Doe
  - For Description write: "I will take this ticket."

![image](https://github.com/user-attachments/assets/986ad149-f716-48f8-9647-3ba2fe3f9cfe)

>[!NOTE]
> It is important to always keep the customer updated even if it is something small. Its best to give the customer consistent updates to make sure they feel taken care of and heard.

- Lets update Karen on the issue
- Scroll down to the "Post Reply" section
- Fill out the reply with: "I suspect the problem might be related to the recent updates. We tested them sufficiently, I am going to look into it further and roll the update back if I determine that was the cause of the outage."

![image](https://github.com/user-attachments/assets/cad9c869-44cc-434e-9e53-a3281b205020)

<h2>Resolution</h2>

>[!NOTE]
> We are going to act like the problem was discovered and was actually the update

- Notify Karen again that the update was the issue
- Create another reply
- Fill out the reply with: "It was determined that the root cause was the recent update. We rolled it back, notified the vendor, and are waiting for a proper fix. Online banking should now be back up and running.

![image](https://github.com/user-attachments/assets/ee707b48-5d29-44c3-ab65-5ba6f90a455c)

- Now that the issue has been fixed we can change the ticket status to: "Resolved"

![image](https://github.com/user-attachments/assets/c5fe6f72-bde2-40c7-ad28-41934c87cf00)











