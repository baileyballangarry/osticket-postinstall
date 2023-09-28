<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop Connection
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b>

<h2>Configuration Steps</h2>

<p>
This tutorial illustrates the process for configuring the osTicket system post-installation. 
 
Following the implementation of osTicket from scratch, attention is turned towards system administration and post-installation setup. 
 
Initially, new roles are configured within the help desk by accessing the Admin panel, selecting "Agents", and then "Roles". The first role to be established is the "Supreme Admin". To do so, click on "Add new role" and enter the name of the new role. It is worth noting that when navigating between the Agent and Admin Panels, the title in the top-right corner of the screen will update accordingly.
</p>

<p>
<img src="https://i.imgur.com/BnzCnIX.png" height="80%" width="80%" alt="Adding a new role"/>
</p>

<p>
It is possible to modify the permissions of any role, including the newly established "Supreme Admin" role, which has full permissions. It's important to note that an agent's level of access is determined by their assigned role, meaning not all agents will have unrestricted access. If the instructions have been followed correctly, the resulting screen should resemble the one depicted. As illustrated, the setup of the "Supreme Admin" role was successful.
</p>

<p>
<img src="https://i.imgur.com/hAKdNgf.png" height="80%" width="80%" alt="Surpreme Admin Role Established"/>
</p>

<p>
While in the Admin Panel, navigate to the Agents tab and locate the "Departments" button. This section allows the creation of new departments, with each Agent being assigned to a specific department based on their role within the helpdesk. In this particular case, a new department called "System Administrators" will be created, and the Supreme Admins will be identified here. Within the departments tab, it is possible to customize specific parameters such as Service Level Agreements (SLAs), managers, and other email preferences.
</p>

<p>
<img src="https://i.imgur.com/xPUwQ5x.png" height="80%" width="80%" alt="System Administrators Department"/>
</p>

<p>
Once a new department has been configured, it is possible to establish a new team. Teams enable the assembly of agents from multiple departments. For instance, one could assemble an "A" team comprising the best technicians from a specific department. Furthermore, support topics can be assigned to a group of agents with relevant expertise in a particular product. To create a team, navigate to Agents -> Teams. In this particular case, a Level II support team will be formed, as a default Level I support team has already been established.
</p>

<p>
<img src="https://i.imgur.com/jg4LlnE.png" width="80%" alt="New Team"/>
</p>

<p>
Now that a new team has been established, we will create a new setting to enable anyone to create tickets. Admin Panel > Settings > User Settings <br />
Ensure that “require registration and login to create tickets” is turned off, this is important for any user to be able to create a ticket.
</p>

<p>
<img src="https://i.imgur.com/t426RLW.png" width="80%" alt="Allowing any user to create a ticket"/>
</p>

<p>
The next step is to create Agents, who are responsible for resolving tickets within the helpdesk. Agents are typically assigned a primary department and position when tickets are routed to a department. While agents may be granted access to other departments, their responsibilities may differ based on their primary department. Within the Agents tab, it is possible to assign Teams, Access, and Permissions. To create Agents, navigate to the Admin Panel, select Agents, and click "Add new agent" to create new Agents as desired.
</p>

<p>
<img src="https://i.imgur.com/vLal9IA.png" height="80%" width="80%" alt="Creating an agent"/>
</p>

<p>
<img src="https://i.imgur.com/FjfDrwD.png" width="80%" alt="Agent acess"/>
</p>

<p>
<img src="https://i.imgur.com/szb9iqJ.png" height="80%" width="80%" alt="Agent team"/>
</p>

<p>
Upon clicking "Create", the newly created Agents should appear as shown in the following image.
</p>
 
<p>
<img src="https://i.imgur.com/MWYXO0T.png" height="80%" width="80%" alt="New Agents"/>
</p>

<p>
After creating Agents, the next step is to create Users, who are clients that submit tickets when they encounter problems. A User is identified by their email address. Follow the steps below to create a User:

Navigate to the Agent Panel, select Users, and click on "User Directory".
Click "Add User" to create a new User or Users.
After creating one or more Users, the User Directory should appear as shown in the following image:
</p>

<p>
<img src="https://i.imgur.com/o7bzRnF.png" height="80%" width="80%" alt="New users"/>
</p>

<p>
SLA Plans define the expected time frame within which a particular ticket is to be resolved by the help desk. To create SLA Plans, navigate to the Admin Panel and select "Manage" followed by "SLA Plans". Each SLA Plan consists of a schedule and a grace period. For example, the SEV-A SLA Plan may have a 24/7 schedule with an hour-long grace period.
</p>

<p>
<img src="https://i.imgur.com/ESyO8KP.png" height="80%" width="80%" alt="Creating an SLA Plan"/>
</p>

<p>
Here is an example of how different SLA Plans can look
</p>

<p>
<img src="https://i.imgur.com/R5SQkEt.png" height="80%" width="80%" alt="Different SLAS"/>
</p>

<p>
Help Topics enable Users to organize their tickets based on specific issues they are experiencing. For instance, if a User is unable to access mobile banking, a relevant Help Topic may be "Business Critical Outage", which can be accessed from the following location:
</p>

<p>
<img src="https://i.imgur.com/Xe00YPw.png" height="80%" width="80%" alt="Help Topic"/>
</p>

<p>
Throughout this tutorial, we have acquired the necessary skills to construct roles, departments, and teams, and assign agents to each one of them. Additionally, we have been introduced to the process of granting varying levels of permissions to different roles and users. Furthermore, we have understood the mechanism of creating users who can access the helpdesk and initiate ticket requests. It is important to understand the interaction between users and agents in a helpdesk environment to gain a comprehensive understanding of its functioning. With the knowledge acquired, you should now have the ability to configure your helpdesk as per your requirements.
</p>
