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

"Switching Between Agent Panel and Admin Panel"

1) After installing osTicket, it's time to configure it as a ticketing system. Keep in mind that the Admin and Agent panels have different configuration settings. To determine which panel you're using, check the top right corner of the osTicket interface. If it shows Agent Panel, you're in the Admin panel, and vice versa.

*Agent Panel:

<p>
<img src="https://imgur.com/VT9lnZl.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  
*Admin Panel:

<p>
<img src="https://imgur.com/042hfd8.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

"Creating the Supreme Admin Role"

2) The second step is to create a new role called Supreme Admin. For this lab, I will create a role with all available permissions. To do so, open the Admin panel, navigate to the Agents menu, click on Roles, and create the new role from there.

</p>
<br />
*Role Name: Supreme Admin
<p>
<img src="https://imgur.com/xgna570.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
*Give Supreme Admin Role all of the tickets permissions
  <p>
<img src="https://imgur.com/dEHltzr.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
*Give Supreme Admin Role all of the tasks permissions
  <p>
<img src="https://imgur.com/4HJhL0E.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
*Give Supreme Admin Role all of the knowledgebase permissions
  <p>
<img src="https://imgur.com/jO8MfHR.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
*Final product of "Supreme Admin"
  <p>
<img src="https://imgur.com/UeDqYQh.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

  
"Configuring Departments (Ticket Visibility, Help Desk, SysAdmins, Networking)"

3) Navigate to Admin Panel -> Agents -> Departments to configure departments such as SysAdmins, which will determine ticket visibility for different teams like Help Desk and Networking.
</p>
<br />
*Leave everything default
<p>
<img src="https://imgur.com/VIuVWUh.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
* Finished the SysAdmin part
  <p>
<img src="https://imgur.com/DdIrX3y.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  
"Configuring Teams"

4) Navigate to Admin Panel -> Agents -> Teams to create teams by pulling agents from different departments, such as forming an Online Banking team.

</p>
<br />

*Leave everything default
<img src="https://imgur.com/afmskYB.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
*This is the finished product for teams
  <p>
<img src="https://imgur.com/LhFgNV3.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  
"Allowing Ticket Creation by Registered Users Only"

5) Navigate to Admin Panel -> Settings -> User Settings and UNCHECK the option that allows unregistered users to create tickets. This ensures that registration and login are required before users can submit tickets.
   
</p>
<br />

<p>
<img src="https://imgur.com/sPVvu6t.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>


"Configuring Agents (Workers)"

6) Navigate to Admin Panel -> Agents -> Add New to configure agents. For example, add Jane to the SysAdmins department and John to the Support department.

</p>
<br />

<p>
<img src="https://imgur.com/qqSZQlo.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

  <p>
<img src="https://imgur.com/jABMfYE.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

 <p>
<img src="https://imgur.com/ltsbLNP.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
  
Service Level Agreements (SLAs) will have to be made in order to categorize tickets according to their level of impact. To make new SLAs, enter the Admin panel and open the Manage menu. Click on SLA and create any needed SLAs. In this case, SEV-A, B, and C have been created to categorize tickets that need to be resolved within 1 hour, 4 hours, and 8 hours respectively.
</p>
<br />

<p>
<img src="https://i.imgur.com/v3zTkfy.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
Finally, Help Topics need to be created to help users select an appropriate category that describes their problem so that Agents get an idea of what problem is described in the ticket. To make a new Help Topic, enter the Admin panel and open the Manage menu. Click on Help Topics and click on Add New Help Topic. In this case, I have added the following in order to use later for when I create new tickets to resolve: Business Critical Outage, Personal Computer Issues, Equipment Reset, and Password Request.
</p>
<br />

<h2>osTicket Configurations are Complete </h2>

Now that the configurations have been set in place, I can now utilize osTicket as a proper ticketing system. I can create tickets and be able to traige them as if I were in a real environment.
