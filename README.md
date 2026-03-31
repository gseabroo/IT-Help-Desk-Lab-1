# IT-Help-Desk-Lab-1
I built a hands-on IT help desk lab using a Windows virtual machine. I used command-line tools to manage user accounts, reset passwords, and simulate account lockouts. I configured file permissions using icacls, troubleshot network issues using ipconfig and ping, and simulated hardware failures by disabling network interfaces. I documented everything in a GitHub repository with screenshots.

# Screenshots
##  Step 1 - Created User Accounts
### Below in this screenshot, you will observe that I ran the 'net user' command to create three user accounts and assigned each one with their own seperate password.
! [Created Users](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Created%20Users.png)

## Administrator JDoe
### Once I made the accounts, they all became standard users by default. I then assigned assigned user JDoe as an administrator within the system.
! [Admin JDoe](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Admin%20jdoe.png)

## Standard User
### This is confirmation that the user is a standard user within the system.
! [Standard TestUser](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Standard%20testuser.png)

## Step 2 - Simulate Account Issues
### From the first screenshot, you can see on the left side of the screen that I have three users: jdoe, asmith and testuser.
! [User Accounts](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/User%20Accounts.png)

### Then I ran the "net user' command and that allowed me to deactivate the user name jdoe. There is proof that the command worked successfully when you look and see that jdoe isn't a viable user anymore.
! [Deactivate](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Deactivate.png)
! [No JDoe](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/No%20Jdoe.png)

### After I confirmed that the command was successful, I then ran another 'net user' command to reactivate the account of JDoe. I also then gave JDoe a completely new password.
! [Activate](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Activate.png)
! [Password Reset](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Password%20Reset.png)

### Once I reset the password, I tried to use the old password to see if the command worked and it was successful. I then used the new password to login and it was successful which you can see by the second screenshot.
! [Failed Login](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Failed%20Login.png)
! [Successful Login](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Succesful%20Login.png)

## Step 3 - Simulate Hardware Issue
### You can see that I ran the 'netsh' command that shows me the name of my interface, what state it is in, what type of interface it is and if it is enabled or not.
! [Interface Name](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Interface%20Name.png)

### I then ran the 'netsh' command that allowed me to disable the interface. Shortly after, I tested the 'ping' command to see if the command had worked successfully and you can see that it did. Once I confirmed that it worked, I enabled the interface and ran the ran command again. The ping command was successful the second time around.
! [Ping Results](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/PIng%20Results.png)

## Step 4 - Network Troubleshooting
### I ran the 'ipconfig' command to show what my IPv4 address, subnet mask and default gateway are that is attached to my network.
! [IpConfig Default](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/IpConfig%20Default.png)

### I then used the 'netsh' command to manually set up my IPv4 address, subnet mask and defauklt gateway. Once I manually set those up, I used the 'ping' command to see if I could reach Google (8.8.8.8) with the manual addresses I gace my network. The 'ping' command was unsuccesful.
! [IpConfig Manual](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/IpConfig%20Manual.png)

### Once I saw that the 'ping' command was unsuccessful, I used the 'netsh' command to use DHCP to automatically assign my IP address and network configuration. Once the command was ran, my addresses were set back to their defaults. I ran the 'ping' command again and it was successful.
! [Successful Ping](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Successful%20Ping.png)
