<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://youtu.be/zNs5ULz1ZwU)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Log into the Admin Panel via http://localhost/osTicket/scp/login.php and direct users to the client portal at http://localhost/osTicket.
- In the Admin Panel, configure Roles, Departments, and Teams to manage agent permissions, visibility, and cross-department collaboration.
- Adjust User Settings to require registration before users can create tickets by unchecking the "unregistered users" option.
- Add Agents under the Admin Panel (e.g., Spongebob in SysAdmins, Patrick in Support) and create Users under the Agent Panel (e.g., Eugene Krabs).
- Set up SLA plans and define Help Topics to organize ticket types and response expectations based on issue severity.

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/8b5c1e75-f17e-4908-814d-19dccd623deb" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  <img src="https://github.com/user-attachments/assets/75f34990-c9e7-4f3b-846d-a9a563fb21b4\" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
</p>
<p>
After installing osTicket, administrators and support agents log in through the Admin Panel at http://localhost/osTicket/scp/login.php, which provides access to system settings and ticket management tools. This is where agents can configure roles, departments, SLAs, and respond to incoming tickets. End users, on the other hand, submit and track their support requests through the client portal at http://localhost/osTicket.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6211ec8e-ebfc-4325-9a3a-cb8b4e2f80e5" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel, go to Agents > Roles to create roles like “Supreme Admin” that define what actions agents can perform. Next, navigate to Agents > Departments to organize agents into groups such as “SysAdmins” or “Support,” which control ticket visibility. Then, under Agents > Teams, create teams like “Online Banking” by combining agents from different departments to collaborate on specific types of issues.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d35b0a05-93b9-47af-8788-5d9f87d5a263" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
To control who can submit support tickets, go to the Admin Panel, then Settings > User Settings. Uncheck the box that allows unregistered users to create tickets, which ensures that only registered users can submit requests. This helps maintain a more secure and manageable ticketing system by requiring user authentication.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/872dec74-5179-47b3-bad1-5bfd5dadbc3a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel, go to Agents > Add New to create agent accounts like Spongebob (assigned to SysAdmins) and Patrick (assigned to Support). Agents are staff members who manage and respond to tickets. To add end users (customers), switch to the Agent Panel, go to Users > Add New, and create profiles for users like Karen and Ken who will submit support requests.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/07861cf4-3fb6-438c-be6f-157bdb91c021" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel, navigate to Manage > SLA to create Service Level Agreements such as Sev-A, Sev-B, and Sev-C, each with different response time expectations and schedules. These SLAs help prioritize tickets based on urgency and ensure timely support. Then go to Manage > Help Topics to create categories like Password Reset or Business Critical Outage, which users select when submitting tickets to streamline routing and handling.
</p>
<br />
