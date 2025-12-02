

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
  <li>Agent accounts (e.g., john and jane)</li>
  <li>Access to the osTicket end-user portal</li>
</ul>

<h2>Deployment Steps</h2>

<h3>Step 1: Access the Admin and End User Panels</h3>
<img src="" width="80%" />
<p>
Open a browser inside the VM and access the osTicket Admin Panel and End User Portal. 
Log in with your administrator or agent accounts. Keep both tabs open to switch between the roles easily.
</p>

<h3>Step 2: Modify Departments</h3>
<img src="" width="80%" />
<p>
Go to the Departments section. Set the SysAdmins department as a top-level department. 
Then delete the Maintenance department entirely. This simulates restructuring departments within a help desk environment.
</p>

<h3>Step 3: Create and Work a Critical Online Banking Ticket</h3>
<img src="" width="80%" />
<p>
As an end user, create a ticket reporting that the entire mobile/online banking system is down.
Switch to the agent account “john,” observe the ticket’s properties, and set:
</p>
<ul>
  <li>SLA: Sev-A (1 hour, 24/7)</li>
  <li>Department: Online Banking</li>
</ul>
<p>
Attempt to view or modify the ticket again as john. Then, log in as jane and work the ticket to completion.
</p>

<h3>Step 4: Create an Adobe Upgrade Ticket (Accounting)</h3>
<img src="" width="80%" />
<p>
As an end user, create a ticket stating that the accounting department needs an Adobe upgrade and it is broken.
As john, observe its initial properties, then update:
</p>
<ul>
  <li>SLA: Sev-B (4 hours, 24/7)</li>
  <li>Department: Support</li>
</ul>
<p>
Work the ticket to completion as john.
</p>

<h3>Step 5: Create and Resolve the CFO Laptop Outage Ticket</h3>
<img src="" width="80%" />
<p>
As an end user, submit a ticket reporting that the CFO’s laptop will no longer turn on.
As john, review the ticket’s properties and update:
</p>
<ul>
  <li>SLA: Sev-B (4 hours, 24/7)</li>
  <li>Department: Support</li>
</ul>
<p>
Simulate diagnosing the problem and complete the ticket.
</p>

<h3>Step 6: Escalate Tickets and Examine Permissions</h3>
<img src="" width="80%" />
<p>
Apply appropriate SLAs to all tickets, and assign the most critical one to the SysAdmins department.
Observe how john can no longer view or modify escalated tickets.
Switch to the Admin Panel to give yourself view-access to SysAdmins, then return to the Agent Panel and observe that the ticket is visible but no longer editable.
</p>

<h3>Step 7: Complete All Tickets and Review Email Behavior</h3>
<img src="" width="80%" />
<p>
Verify all tickets are closed or resolved.
Note that in real help desk environments, email integration means users receive email updates whenever tickets are updated. 
They can reply to those emails, and the responses flow back into the ticket system.
</p>

<h3>Step 8: Real-World Ticket Intake Overview</h3>
<img src="" width="80%" />
<p>
In practice, tickets originate from many sources: phone, chat, email, web forms, even hallway conversations.
While fixing issues on the spot is common, it is important to document everything by creating tickets for tracking, accountability, and metrics.
</p>

<h3>Step 9: Additional Practice</h3>
<img src="" width="80%" />
<p>
osTicket contains many more features than what is covered here. 
Explore ticket filters, canned responses, SLA policies, and email settings.
Repeat this lab multiple times to build strong intuition and reinforce your technical skills.
</p>

<h2>Summary</h2>
<p>
In this lab, we simulated real help desk workflows using osTicket running inside a virtual machine.
We practiced ticket creation, triage, escalation, SLA assignment, resolution, and observed permission effects.
This exercise builds foundational help desk experience critical for IT Support and Systems roles.
</p>
