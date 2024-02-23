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

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents
- Configure New Users
- Configure SLAs
- Configure Help Topics

<h2>Configuration Steps</h2>
<br />

<h2>Login</h2>
<li>Log in to osTicket using the credentials you established during the installation process.</li>
<img src="https://i.imgur.com/iseuePm.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<li><b>Note</b>: OsTicket features two panels: Agent and Admin. You can identify which panel you're currently in by checking if the opposite panel is displayed at the upper right-hand corner. </li>
<img src="https://i.imgur.com/oJQr5sG.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<br />


<h2>Configure Roles</h2>
<p>
<li><b>Roles</b> grant certain permissions to agents within a department to which they are assigned </li>
<ol>
  <li>Navigate to Admin Panel</li>
  <li>Go to Agents</li>
  <li>Select Roles</li>
  <img src="https://i.imgur.com/bW1ysez.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
  <li>Create or configure roles as needed, for example:</li>
  <ul>
    <li>Supreme Admin</li>
  </ul>
<img src="https://i.imgur.com/hepI1Oh.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
  <li>Then Select the Permissions tab</li>
  <ul>
    <li>Here, you can assign specific permissions to this role. For our <b>Supreme Admin role</b>, we will check every box under the <b>Tickets</b>, <b>Tasks</b>, and <b>Knowledgebase</b> tabs. Finally, click on <b>Add Role</b> to finish and create the role.</li>
  </ul>
  <img src="https://i.imgur.com/Jyq6LUV.png" height="50%" width="50%" alt="Disk Sanitization Steps"/> 
  <img src="https://i.imgur.com/OoROREz.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</ol>



<h2>Configure Departments</h2>
<li>Departments are needed to route and resolve tickets based on their importance or instructions</li>
<p>
<ol>
  <li>Access Admin Panel</li>
  <li>Click on Agents</li>
  <li>Choose Departments</li>
</ol>
<img src="https://i.imgur.com/EYZaCVL.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<li>Create or modify departments, such as System Administrators</li>
<img src="https://i.imgur.com/zYJmXPG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2>Configure Teams</h2>
<li>Teams in osTicket enable the organization of agents from various departments to address specific issues while superseding the agents' and their departments' parameter rules.</li>
<ol>
  <li>Open Admin Panel</li>
  <li>Select Agents</li>
  <li>Click on Teams</li>
</ol>
<p>
<img src="https://i.imgur.com/jGSigud.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Configure New Team</h2>
<p>
<li> Create or modify teams such as Level I Support or Level II Support </li>
<br />
<img src="https://i.imgur.com/FTBK3ay.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<li>Assign agents to the team</li>
<br />
<img src="https://i.imgur.com/iecVKXQ.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Allow Anyone To Create A Ticket</h2>
<li>In osTicket, administrators can configure the system to allow anyone, including users outside of the organization, to create tickets.</li>
<ol>
  <li>Go to Admin Panel</li>
  <li>Access Settings</li>
  <li>Navigate to User Settings</li>
  <li>Modify Setting</li>
  <ul>
    <li>Enable Registration Required</li>
    <li>Require registration and login to create tickets</li>
  </ul>
</ol>
<br />
<p>
<img src="https://i.imgur.com/8fKUpF9.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<h2>Configure Agent (Workers)</h2>
<p>
<li>Agents (or workers) are granted access to the help desk in osTicket to respond, resolve, and update the status of tickets </li>
<ol>
  <li>Open Admin Panel</li>
  <li> Go to Agents</li>
  <li>Select Add New</li>
<img src="https://i.imgur.com/1EOk0AJ.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>

<li>Add agents, for example</li>
  <ul>
    <li>Jane</li>
  </ul>
<li>Fill in information such as email and click "Set Password" to proceed.</li>
<img src="https://i.imgur.com/wYvKSpM.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>

<li>Set the agent's password and uncheck the "Password Reset Email" box to proceed</li>
<img src="https://imgur.com/5fN5Ajb.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<li>Navigate to the Access tab to set the agent's Primary Department (mandatory for agent creation). Extended Access can also be granted to the agent to provide access to additional departments.</li>
<img src="https://i.imgur.com/1zmkFc2.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</ol> 
</p>
<br />

<h2>Congifure Users (Customers)</h2>
<p>
<li>typically, users are created as tickets are submitted. When a user submits a ticket via the osTicket system, their email address is often captured along with the ticket details. </li>
<li>However, in a practice environment or during testing, it's common to create user accounts manually.</li>
<ol>
  <li>Go to Agent Panel</li>
  <li>Got to Users</li>
  <li> Select User Directory
  <li>Click Add User</li>
</ol>
<img src="https://i.imgur.com/jIvAN72.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/jFSwbWW.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<li>Owners of tickets can track the status of their tickets. Here are some tickets created by Ken and Karen.</li>
<img src="https://i.imgur.com/UDEyyUl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Configure SLA</h2>
<p>
<li>SLA (Service Level Agreement) functionality allows organizations to define and enforce specific response and resolution times for tickets. SLAs help ensure that customer inquiries are addressed promptly and efficiently.</li>
<ol>
  <li>Access Admin Panel</li>
  <li>Go to Manage</li>
  <li>Select SLA.</li>
  <li>Set SLA levels, for example</li>
  <ul>
    <li>Sev-A (1 hour, 24/7)</li>
    <li>Sev-B (4 hours, 24/7)</li>
    <li>Sev-C (8 hours, business hours)</li>
  </ul>
</ol>
<img src="https://i.imgur.com/rF2PUZP.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2> Configure Help Topics</h2>
<p>
<li>Help Topics are essentially categories or classifications that are used to organize and categorize tickets based on the type of issue or inquiry. </li>
  <ol>
    <li>Access Admin Panel</li>
    <li>Go to Manage</li>
    <li>Select Help Topics</li>
    <img src="https://i.imgur.com/ROp5BDo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <li>Create or edit help topics,such as:</li>
    <ul>
      <li>Business Critical Outage</li>
      <li>Personal Computer Issues</li>
      <li>Equipment Request</li>
      <li>Password Reset</li>
      <img src="https://i.imgur.com/04BpUvA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    </ul>
  </ol>
</p>




