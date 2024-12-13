<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configurations</h1>
This lab demonstrates the necessary changes I make to configure osTicket so it can be used as a proper ticketing system.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- osTicket 

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (21H2)


<h2>Configuration Steps</h2>

**Switching Between Agent Panel and Admin Panel**

1.) After installing osTicket, it's time to configure it as a ticketing system. Keep in mind that the Admin and Agent panels have different configuration settings. To determine which panel you're using, check the top right corner of the osTicket interface. If it shows Agent Panel, you're in the Admin panel, and vice versa.

- Agent Panel:

<p>
<img src="https://imgur.com/VT9lnZl.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  
- Admin Panel:

<p>
<img src="https://imgur.com/042hfd8.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

**Creating the Supreme Admin Role**

2) The second step is to create a new role called Supreme Admin. For this lab, I will create a role with all available permissions. To do so, open the Admin panel, navigate to the Agents menu, click on Roles, and create the new role from there.

</p>
<br />
- Role Name: Supreme Admin
<p>
<img src="https://imgur.com/xgna570.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Give Supreme Admin Role all of the tickets permissions
  <p>
<img src="https://imgur.com/dEHltzr.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Give Supreme Admin Role all of the tasks permissions
  <p>
<img src="https://imgur.com/4HJhL0E.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Give Supreme Admin Role all of the knowledgebase permissions
  <p>
<img src="https://imgur.com/jO8MfHR.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Final product of "Supreme Admin"
  <p>
<img src="https://imgur.com/UeDqYQh.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

  
**Configuring Departments (Ticket Visibility, Help Desk, SysAdmins, Networking)**

3) Navigate to Admin Panel -> Agents -> Departments to configure departments such as SysAdmins, which will determine ticket visibility for different teams like Help Desk and Networking.
</p>
<br />
- Leave everything default
<p>
<img src="https://imgur.com/VIuVWUh.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Finished the SysAdmin part
  <p>
<img src="https://imgur.com/DdIrX3y.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  
**Configuring Teams**

4) Navigate to Admin Panel -> Agents -> Teams to create teams by pulling agents from different departments, such as forming an Online Banking team.

</p>
<br />

- Leave everything default
<img src="https://imgur.com/afmskYB.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- This is the finished product for teams
  <p>
<img src="https://imgur.com/LhFgNV3.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  
**Allowing Ticket Creation by Registered Users Only**

5) Navigate to Admin Panel -> Settings -> User Settings and UNCHECK the option that allows unregistered users to create tickets. This ensures that registration and login are required before users can submit tickets.
   
</p>
<br />

<p>
<img src="https://imgur.com/sPVvu6t.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>


**Configuring Agents (Workers)**

6) Navigate to Admin Panel -> Agents -> Add New to configure agents. For example, add Jane to the SysAdmins department and John to the Support department.

</p>
<br />
- Inputted "Full Name", "Full Email", & "Username" for Jane Doe
<p>
<img src="https://imgur.com/qqSZQlo.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Assigned "SysAdmin" & "Supreme Admin"
  <p>
<img src="https://imgur.com/jABMfYE.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Assigned to "Online Banking" Department
 <p>
<img src="https://imgur.com/ltsbLNP.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Inputted "Full Name", "Full Email", & "Username" for John Doe
<p>
<img src="https://imgur.com/ltsbLNP.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Assigned "Support" & "View Only"
<p>
<img src="https://imgur.com/ltsbLNP.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

**Configuring Users (Customers)**

7) Navigate to Agent Panel -> Users -> Add New to configure users. For example, add Karen as customers.
</p>
<br />

<p>
<img src="https://imgur.com/bb4LmTA.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

  <p>
<img src="https://imgur.com/25zdGEe.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>


**Configuring SLA (Service Level Agreements)**

8) Navigate to Admin Panel -> Manage -> SLA to configure Service Level Agreements. For example, create the following SLAs:

- Sev-A: Grace Period: 1 hour, Schedule: 24/7
- Sev-B: Grace Period: 4 hours, Schedule: 24/7
- Sev-C: Grace Period: 8 hours, Schedule: Business Hours
</p>
<br />
*Sev-A*
  <p>
<img src="https://imgur.com/moXSWgB.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- *Sev-B*
  <p>
<img src="https://imgur.com/Ktp4DH5.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- *Sev-C*
  <p>
<img src="https://imgur.com/PPsWNFB.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  <p>
    
  **Configuring Help Topics (For Ticket Creation)**

9) Navigate to Admin Panel -> Manage -> Help Topics to set up categories for users to select when creating a ticket. Examples of help topics include:

- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other
</p>
<br />

- Business Critical Outage
  <p>
<img src="https://imgur.com/qwiJhDe.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Personal Computer Issues
  <p>
<img src="https://imgur.com/tBY0Cb5.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  - Equipment Request
  <p>
<img src="https://imgur.com/kjG1eOd.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  <p>
- Password Reset
  <p>
<img src="https://imgur.com/YTDcEtr.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
- Other
  <p>
<img src="https://imgur.com/pn9ONIK.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>


<h2>osTicket Configurations are Complete </h2>

*Now that the configurations have been set in place, I can now utilize osTicket as a proper ticketing system. I can create tickets and be able to traige them as if I were in a real environment.*
