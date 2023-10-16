<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>

This guide provides instructions for configuring the open-source help desk ticketing system, osTicket, after installation..<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop Connection
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b>

<h2>Configuration Steps</h2>

<p>
This guide demonstrates the steps to set up the program "osTicket" after it has been installed.

After deploying osTicket from the ground up, the focus shifts to system administration and the configuration that follows.

To begin, the process involves creating new roles within the help desk. This is done by accessing the Admin panel, clicking on "Agents," and then selecting "Roles." The initial role to create is the "Supreme Admin." To accomplish this, click on "Add new role" and provide a name for the new role. It's worth noting that as you navigate between the Agent and Admin Panels, the title in the top-right corner of the screen will be updated accordingly.
</p>

<p>
<img src="https://i.imgur.com/BnzCnIX.png" height="80%" width="80%" alt="Adding a new role"/>
</p>

<p>
You can adjust the permissions for any role, even the recently created "Supreme Admin" role, which has complete permissions. It's crucial to understand that an agent's level of access is determined by their assigned role, so not all agents will have unrestricted access. If the instructions have been correctly followed, the resulting screen should mirror the one shown. This demonstrates that the configuration of the "Supreme Admin" role was successful.
</p>

<p>
<img src="https://i.imgur.com/hAKdNgf.png" height="80%" width="80%" alt="Surpreme Admin Role Established"/>
</p>

<p>

When you're within the Admin Panel, go to the Agents tab and find the "Departments" button. This section enables the establishment of new departments, where each Agent can be assigned to a particular department corresponding to their role in the helpdesk. In this specific scenario, a fresh department named "System Administrators" will be generated, and it's in this department that the Supreme Admins will be designated. Within the departments tab, you have the flexibility to tailor specific settings such as Service Level Agreements (SLAs), managerial roles, and other email preferences.
</p>

<p>
<img src="https://i.imgur.com/xPUwQ5x.png" height="80%" width="80%" alt="System Administrators Department"/>
</p>

<p>
After configuring a new department, you can create a new team. Teams allow you to gather agents from various departments. For instance, you could create an "A" team by selecting the top technicians from a specific department. Additionally, you can assign support topics to a group of agents with expertise in a specific product. To establish a team, go to Agents -> Teams. In this particular instance, we will create a Level II support team, as a Level I support team has already been set up as the default.
</p>

<p>
<img src="https://i.imgur.com/jg4LlnE.png" width="80%" alt="New Team"/>
</p>

<p>
 With the new team in place, let's configure a setting that allows anyone to create tickets. Go to the Admin Panel > Settings > User Settings. <br />
Make sure to disable "require registration and login to create tickets." This step is crucial to enable any user to create a ticket.
</p>

<p>
<img src="https://i.imgur.com/t426RLW.png" width="80%" alt="Allowing any user to create a ticket"/>
</p>

<p>
The next task involves the establishment of Agents, who are responsible for addressing helpdesk tickets. Agents are usually affiliated with a primary department and a designated role for ticket routing. Although agents might be authorized to access multiple departments, their duties may vary according to their primary department. In the Agents section, you have the capability to allocate Teams, Access, and Permissions. To generate Agents, proceed to the Admin Panel, select Agents, and select the "Add new agent" option to create Agents as needed.
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
Once you've set up Agents, the next task is to establish Users, individuals who will submit tickets when they encounter issues. Each User is associated with their email address. To create a User, follow these steps:

Go to the Agent Panel, choose "Users," and then click on "User Directory."

Click "Add User" to generate one or multiple Users.

After creating one or more Users, the User Directory should look like the image provided below:
</p>

<p>
<img src="https://i.imgur.com/o7bzRnF.png" height="80%" width="80%" alt="New users"/>
</p>

<p>
SLA Plans establish the anticipated time frame in which a specific ticket should be resolved by the help desk. To craft SLA Plans, access the Admin Panel, and select "Manage," then choose "SLA Plans." Each SLA Plan comprises a timetable and an allowance period. For instance, the SEV-A SLA Plan might feature a 24/7 schedule with a one-hour grace period.
</p>

<p>
<img src="https://i.imgur.com/ESyO8KP.png" height="80%" width="80%" alt="Creating an SLA Plan"/>
</p>

<p>
Here's an image showcasing the various appearances of different SLA Plans.
</p>

<p>
<img src="https://i.imgur.com/R5SQkEt.png" height="80%" width="80%" alt="Different SLAS"/>
</p>

<p>
Help Topics allow Users to categorize their tickets according to the specific problems they encounter. For example, if a User is facing issues with mobile banking access, they can choose the appropriate Help Topic, such as "Business Critical Outage," accessible from the following location:
</p>

<p>
<img src="https://i.imgur.com/Xe00YPw.png" height="80%" width="80%" alt="Help Topic"/>
</p>
Throughout this tutorial, we've developed the essential skills to establish roles, departments, and teams, and allocate agents to these entities. We've also gained knowledge into the understandings of different permission levels to various roles and users. Furthermore, we've gained insight into the process of creating users who can access the helpdesk and initiate ticket requests.

Understanding the interaction between users and agents within a helpdesk environment is key for a comprehensive understanding of its operation. With this knowledge at your disposal, you should now be well-equipped to configure your helpdesk according to your specific needs.
<p>

</p>
