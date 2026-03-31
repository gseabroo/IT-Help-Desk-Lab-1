# IT-Help-Desk-Lab-1
I built a hands-on IT help desk lab using a Windows virtual machine. I used command-line tools to manage user accounts, reset passwords, and simulate account lockouts. I configured file permissions using icacls, troubleshot network issues using ipconfig and ping, and simulated hardware failures by disabling network interfaces. I documented everything in a GitHub repository with screenshots.

# Screenshots
##  Step 1 - Created User Accounts
### Below in this screenshot, you will observe that I ran command prompt as an administrator and you will see that I created three user accounts and assigned each one with their own seperate password.
! [Created Users](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Created%20Users.png)

## Administrator JDoe
### Once I made the accounts, they all became standard users by default. I then assigned assigned user JDoe as an administrator within the system.
! [Admin JDoe](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Admin%20jdoe.png)

## Standard User
### Once I made the accounts, they all became standard users by default. This is confirmation that the user is a standard user within the system.
! [Standard TestUser](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Standard%20testuser.png)

## Step 2 - Simulate Account Issues
### From the first screenshot, you can see on the left side of the screen that I have three users: jdoe, asmith and testuser.
! [User Accounts](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/User%20Accounts.png)

### Then I ran a command that allowed me to deactivate the user name jdoe. There is proof that the command worked successfully when you look and see that jdoe isn't a viable user anymore.
! [Deactivate](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/Deactivate.png)
! [No JDoe](https://github.com/gseabroo/IT-Help-Desk-Lab-1/blob/main/No%20Jdoe.png)

### After I confirmed that the command was successful, I then ran a seperate command to reactivate the account of JDoe. I also then gave JDoe a completely new password.
! [Activate]()
! [Password Reset]()

### Once I reset the password, I tried to use the old password to see if the command worked and it was successful. I then used the new password to login and it was successful which you can see by the second screenshot.
! [Failed Login]()
! [Successful Login]()
