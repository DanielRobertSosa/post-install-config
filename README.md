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
🔑 Accessing osTicket
  
- Admin Panel – Log in at http://localhost/osTicket/scp/login.php to manage settings, roles, departments, SLAs, and tickets.
- Client Portal – End users go to http://localhost/osTicket to submit new requests and track existing tickets.

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
<img width="976" height="748" alt="image" src="https://github.com/user-attachments/assets/a94ba4c6-0530-4036-a622-9d9207c5f331" />

</p>
<p>
👥 Agents & Users

- Agents – In the Admin Panel → Agents → Add New, create staff accounts (e.g., Dan in SysAdmins, Robert in Support) to manage and respond to tickets.
- Users – In the Agent Panel → Users → Add New, create end-user profiles (e.g., Jane, John) who submit support requests through the client portal.
  
</p>
<br />

<p>
<img width="1203" height="478" alt="image" src="https://github.com/user-attachments/assets/5ba9e960-4564-445b-a5a3-dcc81957d208" />

</p>
<p>
⏱️ SLA Plans & Help Topics

- SLA Plans
  - Go to Admin Panel → Manage → SLA.
  - Create service levels (like Sev-A, Sev-B, Sev-C).
  - Each level should have different response times so urgent tickets get handled faster.

<img width="952" height="725" alt="image" src="https://github.com/user-attachments/assets/ac60a2d6-0195-482b-9755-1f7922ae685a" />

- Help Topics
  - Go to Admin Panel → Manage → Help Topics.
  - Add categories such as Password Reset or Business Critical Outage.
  - Users pick a topic when they submit a ticket, which helps the system send it to the right team.
