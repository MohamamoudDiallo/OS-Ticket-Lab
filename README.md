<h1>osTicket Ticket Management Lab (Running Inside an Azure VM)</h1>
<p>
In this lab, we will use an osTicket installation running inside a virtual machine to simulate real Help Desk operations. 
We will create tickets as end users, update and resolve them as agents, adjust departments and SLAs, and observe how permissions impact ticket visibility.
</p>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machine hosting osTicket)</li>
  <li>osTicket (Help Desk Ticketing System)</li>
  <li>Web Browser (Chrome / Edge)</li>
</ul>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 / 11 (local computer)</li>
  <li>Windows 10 / Windows Server (VM running osTicket)</li>
</ul>

<h2>Prerequisites</h2>
<ul>
  <li>Access to an Azure VM with osTicket installed</li>
  <li>Admin login for osTicket</li>
  <li>Agent accounts </li>
  <li>Access to the osTicket end-user portal</li>
</ul>

<h2>Deployment Steps</h2>

<h3>Step 1: Access the Admin and End User Panels</h3>
<p>Screenshot: <a href="https://imgur.com/a/EPZptqC" target="_blank">View Image</a></p>
<p>
Open a browser inside the VM and access the osTicket Admin Panel and End User Portal. 
Log in with your administrator or agent accounts.
</p>

<h3>Step 2: Modify Departments</h3>
<p>Screenshot: <a href="https://imgur.com/a/sBQRxQE" target="_blank">View Image</a></p>
<p>
From the Admin Panel, go to the Departments section. Set the SysAdmins department as a top-level department. 
Then delete the Maintenance department entirely. This simulates restructuring departments within a help desk environment.
</p>

<h3>Step 3: Create and Work a Critical Online Banking Ticket</h3>
<p>Screenshot: <a href="https://imgur.com/a/MKlkY8f" target="_blank">View Image</a></p>
<p>
As an end user, create a ticket reporting that the entire mobile/online banking system is down.
Switch to the agent account “john,” locate the ticket, and observe its properties (priority, department, SLA, and assignee). Then set:
</p>
<ul>
  <li>SLA: Sev-A (1 hour, 24/7)</li>
  <li>Department: Online Banking</li>
</ul>
<p>

</p>

<h3>Step 3.1: Update SLA and Confirm Ticket Properties</h3>
<p>Screenshot: <a href="https://imgur.com/a/xG3kgdi" target="_blank">View Image</a></p>
<p>
Update the ticket’s SLA to Sev-A and verify that the correct department and priority are set.
Confirm that the ticket reflects the new SLA and department configuration.
</p>

<h3>Step 4: Assign, Resolve the Ticket, and Review Email Behavior</h3>
<p>Screenshot 1: <a href="https://imgur.com/a/XmfIU3F" target="_blank">View Image</a></p>
<p>Screenshot 2: <a href="https://imgur.com/a/91yMHC0" target="_blank">View Image</a></p>
<p>
As the agent, assign the ticket to the appropriate person or team and add an internal note explaining that you are taking ownership of the issue.
Work the ticket through its lifecycle until the problem is resolved, then close the ticket.
In a real help desk environment, email integration ensures that end users receive updates whenever the ticket is updated or closed. Users can reply directly to those emails, and their responses are captured inside the ticket thread.
</p>

<h2>Summary</h2>
<p>
In this lab, we simulated real help desk workflows using osTicket running inside a virtual machine.
We practiced ticket creation, triage, SLA assignment, agent assignment, resolution steps, and observed how ticket updates reflect in the system.
This exercise builds foundational help desk experience that is critical for IT Support and Systems roles.
</p>
