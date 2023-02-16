<p align="center">
    <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket Post Install Configuration

This tutorial outlines the post install configuration of the open-source help desk ticketing system osTicket.

## Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

## Operating Systems Used

- Windows 10 (21H2)

## List of Prerequisites

- Azure Virtual Machine

## Installation Steps

![azure](https://i.imgur.com/0TDG5uH.png)

- Go to "https:www.portal.azure.com"
- click on VM
- click on osTicket VM
- get ip address
- open remote desk top on your computer
- use the IP address to log in

--- 

![osTicket Login](./adminLogin.png)

- In the VM log into osTicket int he web browser:
    localhost/osTicket/scp/login

---

![Admin Permissions](./adminPermissions.jpeg)

- Go to Admin panel-> Agents-> Roles
- Click add new role
- Name Supreme Admin
- Click Permissions
- Check all boxes under Tickets, Task, and Knowledgebase
- save changes
- now we have role that can do everything

--- 

![Department](./department.jpeg)

- Now lets make a new department
- Go to Admin panel-> Agents-> Departments
- click add new department:
    - Name: System Administrators
    - click Create Dept

--- 

![level 2 support](./level2Support.jpeg)
![team members](./teamMembers.jpeg)

- Now we need to make a team
- go to Admin panel-> Agents-> Teams -> add new team
- Name: Level II Support
- click members
- add yourself
- click create team

---

![create Tickets](./createTickets.jpeg)

- now we need to allow anyone to create tickets
- go to Admin Panel -> Settings -> Users ->Settings
- uncheck Registration Required: Require registration and login to create tickets 

---

![new agent account](./newAgentAccount.jpeg)
![new agent role](./newAgentRole.jpeg)
![new agent teams](./newAgentTeams.jpeg)

- Now we need to create agents
- agents are teh help desk professionals
- go to Admin Panel -> Agents -> Add New
- add the information for the agents
- go to access and make them:
    - Department: System Admin
    - Role: Supreme Admin
- go to team
    - select the team you want
    - click add
- click create
- add all the team members you need

---

![click agent panel](./clickAgentPanel.jpeg)
![click add user](./clickAddUser.jpeg)

- now lets create some users. 
    - In osTicket users are the customers that can create tickets
    - they one the tickets they create
- go to Agent Panel -> Users -> Add New
- add the user's information
- click add user to save

---

![user to SLA](./usertoSLA.jpeg)
![create SLA](./createSLA.jpeg)

- Now we need to set up SLAs
- go to Admin Panel -> Manage -> SLA
- click add new
- make the SLAs you need for your organization
    - general SLAs:
        - Sev-A (1 hour, 24/7)
        - Sev-B (4 hours, 24/7)
        - Sev-C (Monday - Friday 8am - 5pm with U.S. Holidays)

---

![add help topics](./helpTopics.jpeg)

- Now we need to ad some general help topics so the users can categorize what they need help with
- Go to Admin Panel -> Manage -> SLA
- click ad new
- add the topics you need for your organization
- general help topics:
    - Business Critical Outage
    - Personal Computer Issues
    - Equipment Request
    - Password Reset





![osTicket Login](./adminSettings.jpeg)


![alt text](https://i.imgur.com/XHteqdt.png")

--- 
![alt text](https://i.imgur.com/dGK0RVM.png")
![alt text](https://i.imgur.com/cYzWBD2.png")
![alt text](https://i.imgur.com/H1q2Fdh.png")
![alt text](https://i.imgur.com/8WTOSre.png")
![alt text](https://i.imgur.com/xOprA9f.png")
![alt text](https://i.imgur.com/LpjCaLd.png")
![alt text](https://i.imgur.com/kB7rts2.png")
