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
