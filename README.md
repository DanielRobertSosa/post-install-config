<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. The configuration ensures proper role management, user access, and structured ticket workflows to support IT service operations.





<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

Access & Navigation
- Log into the Admin Panel via http://localhost/osTicket/scp/login.php.
- Direct end-users to the Client Portal at http://localhost/osTicket.

Agent & Department Management
- Configure Roles, Departments, and Teams in the Admin Panel to control agent permissions, ticket visibility, and enable cross-department collaboration.
- Add Agents (e.g., Dan in SysAdmins, Robert in Support), Create Users under the Agent Panel (e.g., Dan Sosa) for ticket submission.
- Set up SLA plans and define Help Topics to organize ticket types and response expectations based on issue severity.

User Settings
- Require registration before ticket creation by disabling the “unregistered users” option.

Ticket Workflow Setup
- Create SLA Plans to set response and resolution expectations.
- Define Help Topics to categorize tickets and streamline issue routing (based on severity or type).


<h2>Configuration Steps</h2>

🔐 Admin Panel

<img width="1477" height="968" alt="image" src="https://github.com/user-attachments/assets/1f355a2d-3969-4e33-b9b4-5cffaeabdf62" />


🧑‍💻 Agent Panel

<img width="991" height="402" alt="image" src="https://github.com/user-attachments/assets/b3c63638-0429-49f6-a632-853f7a5bf36f" />

  
</p>
<p>
After installation, administrators and agents log in via the Admin Panel (http://localhost/osTicket/scp/login.php) to manage system settings, roles, departments, SLAs, and tickets. End users access the Client Portal (http://localhost/osTicket) to submit and track their support requests.
</p>
<br />

<p>
<img width="963" height="689" alt="image" src="https://github.com/user-attachments/assets/b0ad4a6b-8a0e-452e-a819-a42a2ff48e68" />

</p>
<p>
⚙️ Admin Panel: Roles, Departments, and Teams
  
- Roles – Define agent permissions (e.g., Supreme Admin with full access).
- Departments – Group agents (e.g., SysAdmins, Support) to manage ticket visibility.
- Teams – Combine agents across departments (e.g., Online Banking) for cross-functional collaboration.
</p>
<br />

<p>
<<img width="962" height="502" alt="image" src="https://github.com/user-attachments/assets/8be31d00-e442-4427-88f1-5ec8a2382cd7" />


</p>
<p>
🔐 User Settings
  
- Navigate to Admin Panel → Settings → User Settings.
- Uncheck the option for unregistered users to create tickets.
- This ensures only registered users can submit requests, improving security and maintaining a manageable ticketing system.

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/872dec74-5179-47b3-bad1-5bfd5dadbc3a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel, go to Agents > Add New to create agent accounts like Dan (assigned to SysAdmins) and Robert (assigned to Support). Agents are staff members who manage and respond to tickets. To add end users (customers), switch to the Agent Panel, go to Users > Add New, and create profiles for users like Jane and John who will submit support requests.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/07861cf4-3fb6-438c-be6f-157bdb91c021" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel, navigate to Manage > SLA to create Service Level Agreements such as Sev-A, Sev-B, and Sev-C, each with different response time expectations and schedules. These SLAs help prioritize tickets based on urgency and ensure timely support. Then go to Manage > Help Topics to create categories like Password Reset or Business Critical Outage, which users select when submitting tickets to streamline routing and handling.
</p>
<br />
