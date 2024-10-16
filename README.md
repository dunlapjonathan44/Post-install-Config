<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

Configuring Roles, Departments and Teams 
- Configuring Agents and users
- Configuring SLA's Sev-A, Sev-B, Sev C
- Configuring Help Topics


<h2>Configuration Steps</h2>

Login as an Admin user at http://localhost/osTicket/scp then click on Admin Panel in the top right then hover over Agents>Roles

<p>
<img src="https://i.imgur.com/XMH3JI7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Each role provides different levels of permissions for the agents we create. The permissions range from View only, where the agent can only view tickets, to All access, which grants full control. Agents with full access can assign tickets, adjust SLA levels, create, close, or delete tickets, and more. To add departments, click on Departments next to the Roles tab, then select Add new department to proceed with the setup.

<img src="https://i.imgur.com/YjBRHVF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<br />

<p>

</p>
<p>

This section allows the creation of different departments within the company, where you can configure unique SLA schedules, assign tickets to specific departments, and set up alerts and auto-responses. After configuring departments, you can proceed to the Teams tab and click Add New Team to assign agents to specialized teams for more efficient ticket management.



<img src="https://i.imgur.com/Rp9mtH5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />

<p>

</p>
<p>Teams can be created within departments to better organize agent roles. For example, you might have an Online Banking team within the SysAdmins department. Once agents are created, team members can be added to handle specific ticket requests. Additionally, users can submit tickets without needing to register an account. To enable this, go to Settings -> Users, and uncheck the option Require registration and login to create tickets. This simplifies the process for users seeking IT support.

<img src="https://i.imgur.com/A4LYFf5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/OKXbzLA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


  Now we can begin adding agents to manage and respond to tickets in the help desk system. To do this, navigate to the Agents tab, and click on Add New Agent. This allows you to input essential details such as the agent's name, email, and role. Assigning agents to specific roles ensures they have the correct permissions to view, manage, or resolve tickets. As you continue, agents can be further assigned to departments or teams, streamlining your ticket workflow for better support coverage.

<img src="https://i.imgur.com/3AJZL8c.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




  We can configure an agent’s details such as their name, password, and email address, while also assigning their access level, permissions, and team. For instance, you could create an agent named Jane Doe, assign her to the SysAdmins department, and grant her All Access. This level of access provides default permissions, but you can customize specific settings if needed. Similarly, you might create John Doe, assign him to the Support department, and grant him Expanded Access to limit permissions while maintaining flexibility in ticket handling.

<img src="https://i.imgur.com/vLRKsWC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  It's a good practice to assign agents to specific teams, enabling them to collaborate and assign tickets to agents in other teams if needed. To do this, go to Teams and add each agent to their respective team. For example, Jane Doe can be assigned to Online Banking, and John Doe to Support. Additionally, you can create users (customers) who need support. Click the Agent Panel in the top right, select Users, and then Add User. In this instance, you can create users named Karen and Ken for demonstration purposes.

<img src="https://i.imgur.com/T96eqau.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

It's essential for agents to prioritize and address tickets based on their urgency and business impact. This can be managed effectively by setting up different SLA (Service Level Agreement) levels. By creating various SLA policies, we can ensure that high-priority tickets receive faster responses and resolutions, while lower-priority issues are handled accordingly. For example, critical issues affecting core systems might have a 1-hour response time, whereas less urgent requests could have a longer resolution window. Customizing SLA levels helps align ticket management with business goals and customer expectations.

<img src="https://i.imgur.com/lLTK3QZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

To create new SLA plans, click on Add New SLA Plan and enter the details according to severity. For example, set Sev-A for the most urgent issues (grace period: 1 hour, schedule: 24x7), Sev-B for medium priority (grace period: 4 hours, schedule: 24x7), and Sev-C for lower priority (grace period: 8 hours, schedule: business hours only). You can also create help topics to categorize incoming tickets more efficiently. While users may not always select the correct category, having options streamlines ticket management. Go to the Admin Panel, click Manage, and then Add New Help Topic.

<img src="https://i.imgur.com/GFxFKyG.png" width="80%" alt="Disk Sanitization Steps"/>

We can now create various help topics to better categorize incoming tickets. Start by choosing a Top-level topic such as Report a Problem. From there, you can create more specific subtopics, like Access Issue, to narrow down the type of request.
</p>
<br />
