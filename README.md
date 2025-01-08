<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Acknowledge the difference between the Agent Panel and Admin Panel.
- Configure Roles to define permissions for agents.
- Set up Departments to group tickets by areas of responsibility.
- Create Teams to pull agents from multiple departments.
- Configure user settings to allow or restrict ticket creation.
- Add Agents (workers) and Users (customers).
- Set up Service Level Agreements (SLAs) for ticket response times.
- Create Help Topics for users to categorize their tickets.

<h2>Configuration Steps</h2>

<h3>1.) Acknowledge Agent Panel vs Admin Panel</h3>

- The **Agent Panel** is used by agents to work on tickets.
- The **Admin Panel** is used to manage system settings, configurations, and permissions.

<h3>2.) Configure Roles</h3>

- Navigate to **Admin Panel -> Agents -> Roles**.
- Add a new role called **Supreme Admin**.
  - Define permissions for agents based on the role they will have. In this lab, we will give permissions for the Tickets, Tasks, and Knowledgebase sections.

![Screenshot 2025-01-07 221906](https://github.com/user-attachments/assets/11794932-b861-450d-a5d4-cbc4397fce90)


![image](https://github.com/user-attachments/assets/b72872bc-d9ec-468c-adc1-596e42b15f3d)


<h3>3.) Configure Departments</h3>

- Navigate to **Admin Panel -> Agents -> Departments**.
- Add a new department called **SysAdmins**.
  - Use departments to control ticket visibility and assign areas of responsibility (e.g., Help Desk, SysAdmins, Networking).

![image](https://github.com/user-attachments/assets/12097558-4d44-43bb-a288-2cdd9db4cc54)


<h3>4.) Configure Teams</h3>

- Navigate to **Admin Panel -> Agents -> Teams**.
- Create a new team called **Online Banking**.
  - Pull agents from different departments to form specialized teams.

![image](https://github.com/user-attachments/assets/f855503a-4f60-4443-8751-89770937975a)


<h3>5.) Allow Anyone to Create Tickets</h3>

- Navigate to **Admin Panel -> Settings -> User Settings**.
- Uncheck **Require registration and login to create tickets** to enforce ticket creation by anyone.
- Enable **Public - Anyone can register** to disable requiring users to register and log in before creating tickets.

![image](https://github.com/user-attachments/assets/cebda212-39f5-4147-94ad-1dabb1cbc0bb)


<h3>6.) Configure Agents (Workers)</h3>

- Navigate to **Admin Panel -> Agents -> Add New**.
- Add agents with the following details:
  - **Jane**: Assigned to the **SysAdmins** department.
  - **John**: Assigned to the **Support** department.

![image](https://github.com/user-attachments/assets/5d71f952-7b7e-49bc-a6c4-4d672e48af5a)


![image](https://github.com/user-attachments/assets/7671cf48-2d2f-4829-babe-336ec9d3061d)


![image](https://github.com/user-attachments/assets/3d8a2d09-3809-49bc-8262-98cf1539f54c)


![image](https://github.com/user-attachments/assets/f27854b3-913c-4bbe-8492-34125f576cd9)


<h3>7.) Configure Users (Customers)</h3>

- Navigate to **Agent Panel -> Users -> Add New**.
- Add users with the following details:
  - **Karen**
  - **Ken**
 
<p>
<img src="https://i.imgur.com/xrJ8gm6.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>8.) Configure SLA (Service Level Agreements)</h3>

- Navigate to **Admin Panel -> Manage -> SLA**.
- Add the following SLAs:
  - **Sev-A**: Grace Period = 1 hour, Schedule = 24/7.
  - **Sev-B**: Grace Period = 4 hours, Schedule = 24/7.
  - **Sev-C**: Grace Period = 8 hours, Schedule = Business Hours.

![image](https://github.com/user-attachments/assets/37799ce9-b7d6-48cd-ad72-d41a86cc1618)


![image](https://github.com/user-attachments/assets/cad59456-de34-42c2-bac4-0d71503a8788)

![image](https://github.com/user-attachments/assets/afbbf66f-4c5e-4521-bf33-c333970549b7)


<h3>9.) Configure Help Topics</h3>

- Navigate to **Admin Panel -> Manage -> Help Topics**.
- Add the following help topics for users to select when creating a ticket:
  - **Business Critical Outage**
  - **Personal Computer Issues**
  - **Equipment Request**
  - **Password Reset**
  - **Other**

![image](https://github.com/user-attachments/assets/0c1d82c1-25fb-428f-b6d5-046a2712951e)


<h2>Conclusion</h2>

By completing the post-installation configuration steps, you have successfully customized osTicket to suit your organization's requirements. You are now ready to start using osTicket to manage and resolve customer issues efficiently.
