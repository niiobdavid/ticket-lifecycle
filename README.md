<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to create, work, and resolves tickets within osTicket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Project Walk-through:</h2>

<h4>Admin/Analyst Login Page:     http://localhost/osTicket/scp/login.php </h4>

<p>
  <img src="https://i.imgur.com/Svhum4U.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>End Users osTicket URL:      http://localhost/osTicket </h4>

<p>
  <img src="https://i.imgur.com/siNMSH3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />
  
<h4>Acknowledge Agent Panel vs Admin Panel</h4>
<p>
  <img src="https://i.imgur.com/iUzb0qq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/MIsuJ4f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />
  
<h4>Configure Roles (for grouping permissions)</h4>

- Admin Panel -> Agents -> Roles
    - Supreme Admin

<p>
  <img src="https://i.imgur.com/Sc5Y8gr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/Th7Ca2I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/q547YJ2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/VmzPYet.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/8BghBkL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/QE5TKro.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)</h4>

- Admin Panel -> Agents -> Departments
    - SysAdmins

<p>
  <img src="https://i.imgur.com/jjGXKo3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/Cu6LNhp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/6iMtkEM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>Configure Teams</h4>

- Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
    - Online Banking

<p>
  <img src="https://i.imgur.com/EtOR2ge.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/mACxyAq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/mjBcvAK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>Allow anyone to create tickets</h4>

- Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
    - Registration Required: Require registration and login to create tickets

<p>
  <img src="https://i.imgur.com/XBjJWQq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>Configure Agents (workers)</h4>

- Admin Panel -> Agents -> Add New
    - Jane (Dept: SysAdmins)
    - John (Dept: Support)

<p>
  <img src="https://i.imgur.com/m0chQA7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/DUUnjqP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/1kLtdrs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/CJWx4VS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/At0fdHK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/HKRMZai.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/GTRPftt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>Configure Users (customers)</h4>

- Agent Panel -> Users -> Add New
    - Karen
    - Ken

<p>
  <img src="https://i.imgur.com/bMurkiz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/oKAQmHg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>Configure SLA</h4>

- Admin Panel -> Manage -> SLA
    - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
    - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
    - Sev-C (Grace Period: 8 hours, Business Hours)

<p>
  <img src="https://i.imgur.com/BeV5CNT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/WrKN8qa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/q5pHGPQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/VjqP1cS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/wSPHw0a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />

<h4>Configure Help Topics (For when users create a ticket)</h4>
- Admin Panel -> Manage -> Help Topics
    - Business Critical Outage
    - Personal Computer Issues
    - Equipment Request
    - Password Reset
    - Other

<p>
  <img src="https://i.imgur.com/cY9YsUL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/45FfhfR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/ZgPTW6M.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/ZgPTW6M.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/58X5iFJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/EAr3vkh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<br />
  
[<h4>Finally done!</h4>
