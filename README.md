<p align="center">
<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/4722ac21b64b314dfb125e002199efe20f965436/images/file%20shares.PNG" width="600" height="200" />
</p>
<h1>Network File Shares and Permissions</h1> 
In this tutorial, file folders will be created within the domain controller, security groups will be created and permissions for users will be set for access

<h1>Environments and Technologies Used</h1>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h1>Operating Systems Used</h1>

Windows 10 (21H2)
Ubuntu Server 20.04
<h1> Steps Overview </h1> 

- Create some sample file shares with various permissions
- Attempt to access file shares as a normal user
- Create an “ACCOUNTANTS” Security Group, assign permissions, an test access


<h1>Create some sample file shares with various permissions</h1>

To begin, some folders will be created and they will each get different permissions. Within the domain controller the following folders will be created within the c-drive.  (“read-access”, “write-access”, “no-access”, “accounting”). Access File Explorer then select the "Windows (C:)" drive. Right click the blank space and select "New" then select "Folder". You can rename this folder by right clicking the folder then selecting "Rename". this folder will be named "read-access".  

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%2040.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%2041.png" width="600" height="400" />

the same steps will be done for the remaining folders.


<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%201.png" width="600" height="400" />


Now that the folders have been created, permissions can be set. The “read-access” folder will get its permissions set first. Right click the “read-access” folder then click on “Properties”. 


<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%202.png" width="600" height="400" />


Within the “Properties” screen, click on the “Sharing” tab on the top left of the screen then click on “Share…” in the middle of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%203.png" width="600" height="400" />


A “Network access” screen will pop-up next. Within this screen,  type in “domain users” in the dropdown text box next to “Add” then click on “Add”.

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%204.png" width="600" height="400" />


Once clicked, “Domain Users” will appear in the box below. The permission level has already been set to “Read” so no changes need to be made. Click on “Share” on the bottom right hand corner.

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%205.png" width="600" height="400" />


The “Network access” screen will appear again with the message “Your folder is shared”. Click on “Done” in the bottom right hand corner of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%206.png" width="600" height="400" />


The same steps will be repeated for the remaining folders. Right click the “write-access” folder then click on “properties”. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%207.png" width="600" height="400" />


Within the “Properties” screen, click on the “Sharing” tab on the top left of the screen then click on “Share…” in the middle of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%208.png" width="600" height="400" />


The “Network access” screen will pop-up next. Within this screen,  type in “domain users” in the dropdown text box next to “Add” then click on “Add”. Click on the drop down menu next to “Read” and select “Read/Write”. Afterwards, Click on “Share” on the bottom right hand corner.

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%209.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%2010.png" width="600" height="400" />


The “Network access” screen will appear again with the message “Your folder is shared”. Click on “Done” in the bottom right hand corner of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/fcd8ebfe853477c387d0806fd2bc4716b2969fbf/images/network%20file%20shares%2011.png" width="600" height="400" />


Permissions will now be given to the “no-access” folder. The “Read/Write” permissions will be given to domain admin users but will not be given to normal users. Because permissions will not be given to normal users, they will not be able to access this folder. The pictures below show all the steps. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/9df774aca4ac570a3677ab30b337d98f5e61914a/images/network%20file%20shares%2012.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/9df774aca4ac570a3677ab30b337d98f5e61914a/images/network%20file%20shares%2013.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2042.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/9df774aca4ac570a3677ab30b337d98f5e61914a/images/network%20file%20shares%2014.png" width="600" height="400" />



The “accounting” folder will not be shared for now. Now that all the folders have been created and permissions have been set, the next section will cover what a normal user on the network will experience when accessing these folders. 

<h1>Attempt to access file shares as a normal user</h1>

As a normal domain user on the network, these folders will be accessed. This will be simulated using a virtual machine that is connected to the network. By typing “\\dc-1” in the search bar within “File Explorer” and pressing enter, the folders that are shared through the network will appear. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2015.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2016.png" width="600" height="400" />

The“read-access” folder can be accessed by the user, but when the user tries to create something within this folder, it is denied. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2017.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2018.png" width="600" height="400" />


The “write-access” folder can be accessed by the user and the user can create contents within it as shown below.

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2019.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2020.png" width="600" height="400" />


Earlier, permissions for the “no-access” folder were given to domain admins, not normal users. So when the “no-access” folder is clicked, the access is denied. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2023.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2024.png" width="600" height="400" />


The “accounting” folder does not show up here because it is not shared within the network.  In the next section a “ACCOUNTANTS” security group will be created and assigned permissions so that the accounting folder can be accessed. 

<h1>Create an “ACCOUNTANTS” Security Group, assign permissions, an test access</h1>

To begin, the Active directory needs to be accessed within the domain controller in order to create the security group. Open “Active Directory Users and Computers” by using the Windows search bar on the bottom left corner of the screen and typing “Active Directory” and clicking on the application.  

<img src="https://github.com/JosephRC777/configure-ad/blob/c8158a0f40f76c07bcabbe0227d6c7c86b433d99/images/Active%20Directory%20DC%20ADmin%201.png" width="600" height="400" />



Within this application, a folder named “_GROUPS” will be created. right click the “mydomain.com” section and select “New” then click on “Organizational Unit”. 

<img src="https://github.com/JosephRC777/configure-ad/blob/c8158a0f40f76c07bcabbe0227d6c7c86b433d99/images/Active%20Directory%20DC%20ADmin%202.png" width="600" height="400" />



A “New Object - Organizational Unit” screen will show up. Within this screen, in the textbox under “Name” the organizational unit can will be given the name “_GROUPS”. After typing the name of the OU, Click on “OK” on the bottom of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2025.png" width="600" height="400" />



Within this “_GROUPS” folder, a new group named “ACCOUNTANTS” will be created. Within the “_GROUPS” folder, right click and select “New” then click on “Group”.

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2026.png" width="600" height="400" />



A “New Object - Group” screen will appear. Within this screen in the textbox under “Group name:” type in “ACCOUNTANTS”. Afterwards, click “OK” on the bottom right hand corner of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2027.png" width="600" height="400" />


Now the “ACCOUNTANTS” security group will appear in the “_GROUPS” folder. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2028.png" width="600" height="400" />


Permissions in the “accounting” folder that was created earlier will now be set to give access to any member in the “ACCOUNTANTS” security group. Within the domain controller, right click the “accounting” folder within the “Windows (C:)” drive and click on “Properties”

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/dc51be297f4c8a23c6c912592d23a8bf99dc5979/images/network%20file%20shares%2029.png" width="600" height="400" />


Within the “Properties” screen, click on the “Sharing” tab on the top left of the screen then click on “Share…” in the middle of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2030.png" width="600" height="400" />


The “Network access” screen will pop-up next. Within this screen,  type in “accountants” in the dropdown text box next to “Add” then click on “Add”.

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2031.png" width="600" height="400" />


Click on the drop down menu next to “Read” and select “Read/Write”. Afterwards, Click on “Share” on the bottom right hand corner.

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2032.png" width="600" height="400" />

The “Network access” screen will appear again with the message “Your folder is shared”. Click on “Done” in the bottom right hand corner of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2033.png" width="600" height="400" />


Now that permissions have been given, a normal user will attempt to access this folder through the network. This should fail since no users have been added to the “ACCOUNTANTS” group. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2034.png" width="600" height="400" />


The normal user will now be added to the “ACCOUNTANTS” security group. Within “Active Directory Users and Computers” click on the “ACCOUNTANTS” security group in the “_GROUPS” folder. A “Properties” screen will show up. Within this screen, click on the 
“Members” tab on the top left corner of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2035.png" width="600" height="400" />


Click on “Add…” on the bottom left corner. In this section a normal user will be selected to be apart of the “ACCOUNTANTS” group. The user “bawa.bib” which was generated using Powershell will be selected. Type the name of the user in the textbox under “Enter the object names to select” section, then click on “Check Names” on the right hand corner of the screen. Afterwards, click “OK” on the bottom of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2036.png" width="600" height="400" />

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2037.png" width="600" height="400" />


The “Properties” screen will show up again. If done correctly, a new user has been added to the group as a member. Click on “Apply” then click on “OK” on the bottom of the screen. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2038.png" width="600" height="400" />


Now, if the added user attempts to access the “accounting” folder within the network, it will be successful. 

<img src="https://github.com/JosephRC777/permissionsandfileshares/blob/f30976cac326f9c551f964325b85f9e61646d732/images/network%20file%20shares%2039.png" width="600" height="400" />


This concludes this network shares and permissions tutorial. 						
