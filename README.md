<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>Deployment and Configuration Steps</h2>
1 If you aren't already Remote Desktop into dc-1 in the Windows App. 
  (I would recommend Remoting into both dc-1 and client-1) 
  To help tell which computer is which the Windows 10 computer will have the windows shopping app on the task bar. 
  The Windows server will not. 
<p>
<p>
<img <img width="1440" alt="DE_1" src="https://github.com/user-attachments/assets/6aff293b-6db8-4558-b8f8-74db3ec3999e" />
</p>
<p>
3 In dc-1 (windows server) right-click start and go to Server Manager. 
<p>
<img <img width="1440" alt="DE_3" src="https://github.com/user-attachments/assets/61972d03-3cf9-4793-92d8-b4adb7cb52d0" />
</p>
<p>
4 If you see this pop up close it. 
<p>
<img <img width="1440" alt="DE_4" src="https://github.com/user-attachments/assets/ad413c40-88d0-4878-8a1d-a104b05f8e12" />
</p>
<p>
5 Click "Add roles and features".
<p>
<img <img width="1440" alt="DE_5" src="https://github.com/user-attachments/assets/09f53e05-00f9-4214-bf10-5e5e74703987" />
</p>
<p>
6 Click "Next".
<p>
<img <img width="1440" alt="DE_6" src="https://github.com/user-attachments/assets/39195262-5ea0-4d21-a77b-e77b569f0080" />
</p>
<p>
7 Click "Next". 
<p>
<img <img width="1440" alt="DE_7" src="https://github.com/user-attachments/assets/ea41713e-ed05-4d63-b5f0-5c96e05e241a" />
</p>
<p>
8 There should only be one server connection for dc-1 and click "Next".
<p>
<img <img width="1440" alt="DE_8" src="https://github.com/user-attachments/assets/05df12a9-e9e8-4d4b-8cef-08dc5f1067c0" />
</p>
<p>
9 Here check the box for "Active Directory Domain Services". 
<p>
<img <img width="1440" alt="DE_9" src="https://github.com/user-attachments/assets/20703338-9285-483a-b605-8238481c2584" />
</p>
<p>
10 This will pop up after you check the box. When it does click "Add Features". 
<p>
<img <img width="1440" alt="DE_10" src="https://github.com/user-attachments/assets/f785c544-40c0-4453-b301-336586ff1681" />
</p>
<p>
11 Click "Next".
<p>
<img <img width="1440" alt="DE_11" src="https://github.com/user-attachments/assets/773d3ef8-0867-48a4-b1c6-8981a47b50b0" />
</p>
<p>
12 Click "Next".
<p>
<img <img width="1440" alt="DE_12" src="https://github.com/user-attachments/assets/78a8488f-dbc6-4a72-b154-464692d7612c" />
</p>
<p>
13 Click "Next". 
<p>
<img <img width="1440" alt="DE_13" src="https://github.com/user-attachments/assets/3fce2d3a-c55a-485c-bd5f-7592da3e23f6" />
</p>
<p>
14 Now check the box for "Restart the Destination server automatically if required and click "yes".
<p>
<img <img width="1440" alt="DE_14" src="https://github.com/user-attachments/assets/0157cedd-1acb-4c47-bec2-734fbf958ba0" />
</p>
<p>
15 Click "Install"
<p>
<img <img width="1440" alt="DE_15" src="https://github.com/user-attachments/assets/ec8bb96d-d856-4f63-85c9-c25405a60be9" />
</p>
<p>
16 After the configuration is complete click "Close".
<p>
<img <img width="1440" alt="DE_16" src="https://github.com/user-attachments/assets/e7d987e0-26a1-4e34-bb0b-0ac6f69f742c" />
</p>
<p>
17 Next we are going to configure dc-1 to become a domain controller by setting up a new forest as mydomain.com.
   In dc-1 at the top right click on the flag and then click "Promote this server to a domain controller". 
<p>
<img <img width="1440" alt="DE_17" src="https://github.com/user-attachments/assets/58389dc1-bfc2-4a25-ad0b-48e2e9bb9561" />
</p>
<p>
19 After this pops up click the circle for "Add a new Forest". For Root domain name: use mydomain.com  
  Click "Next".
<p>
<img <img width="1440" alt="DE_19" src="https://github.com/user-attachments/assets/3bf3d35e-4709-465c-ae69-05294a2b318b" />
</p>
<p>
20 More than likely you won't need this Directory Services Restore password. That being said just set it to something simple like Password1.
   Click "Next".
<p>
<img <img width="1440" alt="DE_20" src="https://github.com/user-attachments/assets/341d1b30-1d67-4ffe-bc01-9adf6cf2e394" />
</p>
<p>
22 If it's checked then uncheck Create DNS delegation. 
   Click "Next".
<p>
<img <img width="1440" alt="DE_22" src="https://github.com/user-attachments/assets/0a72d999-527e-4ef9-adff-2d619d6938a6" />
</p>
<p>
23 Click "Next"
<p>
<img <img width="1440" alt="DE_23" src="https://github.com/user-attachments/assets/cdb7086a-f0a0-419c-9276-398bb2898997" />
</p>
<p>
24 Click "Next"
<p>
<img <img width="1440" alt="DE_24" src="https://github.com/user-attachments/assets/7bcacdf4-db13-450c-91ad-37ee69a34677" />
</p>
<p>
25 Click "Next"
<p>
<img <img width="1440" alt="DE_25" src="https://github.com/user-attachments/assets/a5e7cfad-ba69-46b5-9165-090bfe1a9a8b" />
</p>
<p>
26 Click "Install".
<p>
<img <img width="1440" alt="DE_26" src="https://github.com/user-attachments/assets/2326b4f8-35f1-44f3-b7b5-1d6798a211e4" />
</p>
<p>
27 Now wait for the new forest to be installed. When it is finished it will automatically restart. 
   Click "Close".
<p>
<img <img width="1440" alt="DE_27" src="https://github.com/user-attachments/assets/13dd16ac-0209-44fe-b336-03ba78460756" />
</p>
<p>
28 Click "Close".
<p>
<img <img width="1440" alt="DE_28" src="https://github.com/user-attachments/assets/e3b611e9-5b91-4dd8-b515-7f3016d6a894" />
</p>
<p>
30 Log back into dc-1 but there is a slight change to that process now.
   Now that this is a domain controller the user accounts exist in that domain. 
  Therefore you need to login as mydomain.com\labuser instead of just labuser.
<p>
<img <img width="1440" alt="DE_30" src="https://github.com/user-attachments/assets/86378893-6e3e-4644-a4a9-c0c396fe26cc" />
</p>
<p>
31 Now that we are logged back in we are going to create a domain admin user within the domain. 
   Close the Server Manager Dashboard.
<p>
<img <img width="1440" alt="DE_31" src="https://github.com/user-attachments/assets/177c848e-99c9-4b07-81dc-36593a59ab2c" />
</p>
<p>
32 Click Start at the bottom. 
   Click the drop down arrow for Windows Administrative Tools.
   From there open "Active Directory Users and Computers". 
<p>
<img <img width="1440" alt="DE_32" src="https://github.com/user-attachments/assets/004b4393-b745-48f1-8005-b29aa31ca60b" />
</p>
<p>
33 Expand it and here we will create two Organizational units.
   One named _EMPLOYEES and the other called _ADMINS. 
<p>
<img <img width="1440" alt="DE_33" src="https://github.com/user-attachments/assets/1e285941-3353-47d0-b2e2-e4046d066ab1" />
</p>
<p>
34 Right click mydomain.com, click "New", and click "Organizational Unit".
<p>
<img <img width="1440" alt="DE_34" src="https://github.com/user-attachments/assets/a3ec331a-8c1b-41d5-817f-c07e707b8ee2" />
</p>
<p>
35 For the Name use "_EMPLOYEES". Type it in EXACTLY like that. (IF you dont then you will not be able to perform the following steps.)
  Click "OK".
<p>
<img <img width="1440" alt="DE_35" src="https://github.com/user-attachments/assets/7ee8f96a-cd96-4009-a0d4-b26b8f199438" />
</p>
<p>
36 Do the same process to create another one except name it "_ADMINS". Needs to be exact.
<p>
<img <img width="1440" alt="DE_36" src="https://github.com/user-attachments/assets/d09d4060-0c79-4646-8032-190caa5adf6b" />
</p>
<p>
37 Right click mydomain.com and click "Refresh". 
<p>
<img <img width="1440" alt="DE_37" src="https://github.com/user-attachments/assets/12074c81-47f0-4435-a8a6-bbeb7779845a" />
</p>
<p>
38 Next we are going to create a new user. 
   Click on the _ADMINS folder. 
   Right click open view, then click "New" then "User". 
<p>
<img <img width="1440" alt="DE_38" src="https://github.com/user-attachments/assets/4646df5c-d698-4405-ab12-bf4d55d3e7a8" />
</p>
<p>
39 Fill out
   First name: 
   Last Name: 
   User Logon name: 
   Any name will be fine. Then Click "Next".
<p>
<img <img width="1440" alt="DE_39" src="https://github.com/user-attachments/assets/aa117a28-0abf-4bad-9959-a91d751db5a3" />
</p>
<p>
40 Choose a password you can remember, uncheck "User must change password at next logon", and check the "Password never expires".
   click "Next". 
<p>
<img <img width="1440" alt="DE_40" src="https://github.com/user-attachments/assets/b891d082-a9a1-42c5-bcc9-87ac382fe8ad" />
</p>
<p>
41 Click "Finish".
<p>
<img <img width="1440" alt="DE_41" src="https://github.com/user-attachments/assets/08eb4df0-8280-43dc-b487-f987382e7d7e" />
</p>
<p>
42 Now the first user is created. However this user isn’t an admin just because its in the folder and named as such.
   We need to add this user to the "Domain Admins" Security Group.
<p>
<img <img width="1440" alt="DE_42" src="https://github.com/user-attachments/assets/c1644c54-dd4e-482e-859b-2cb12d3bfea1" />
</p>
<p>
43 Right-click the user and click Properties. 
<p>
<img <img width="1440" alt="DE_43" src="https://github.com/user-attachments/assets/3bfe27f5-a28d-4994-b473-488524a1eae6" />
</p>
<p>
44 Click "Member of".
<p>
<img <img width="1440" alt="DE_44" src="https://github.com/user-attachments/assets/a26102b3-1c11-40c0-b459-713844bdbeae" />
</p>
<p>
45 Click "Add". 
<p>
<img <img width="1440" alt="DE_45" src="https://github.com/user-attachments/assets/2927796c-a273-4b6e-802b-6483f6736465" />
</p>
<p>
46 In the "Enter the object names to select" type "domain admins" and click "Check Names".
<p>
<img <img width="1440" alt="DE_46" src="https://github.com/user-attachments/assets/5923b5a8-d592-4de2-b8a4-f10ac079e781" />
</p>
<p>
47 When it changes to this that means it found Domain Admins built-in group. 
   Click "OK".
<p>
<img <img width="1440" alt="DE_47" src="https://github.com/user-attachments/assets/0b8ca342-d5ea-4f92-88a5-71f62e02486d" />
</p>
<p>
48 Click "Apply" and then "OK". Now this user is a domain admin. 
<p>
<img <img width="1440" alt="DE_48" src="https://github.com/user-attachments/assets/13681512-5001-4612-bcf4-db66388f3de9" />
</p>
<p> 
49 Next we are going to log out. Closing the connection to dc-1 and logging back in as "mydomain.com\jan_admin".
   Right-click start, click run, type "logoff", and click "OK". This will quickly log you out of the vm. 
<p>
<img <img width="1440" alt="DE_49" src="https://github.com/user-attachments/assets/d9ab7105-b2b0-4ce7-94e2-a90eeb9c9352" />
</p>
<p>
50 Log back into dc-1 as the admin you created. 
<p>
<img <img width="1440" alt="DE_50" src="https://github.com/user-attachments/assets/acaba768-0fa1-482a-bb79-f81259e2fc4f" />
</p>
<p>
51 Close the dashboard. 
   Next we will join client-1 to the domain. 
<p>
<img <img width="1440" alt="DE_51" src="https://github.com/user-attachments/assets/c0bdea20-f650-4fd4-bd90-0faefee2eea1" />
</p>
<p>
52 If you havent already get the public IP address for client-1 and sign in as the user you created. 
<p>
<img <img width="1257" alt="Screenshot 2025-07-04 at 1 15 55 PM" src="https://github.com/user-attachments/assets/755f1c05-2a07-44a9-8686-49390d8d0914" />
<p>
53 When you are logged in right click the start menu and click "System". 
<p>
<img <img width="1268" alt="Screenshot 2025-07-04 at 1 19 18 PM" src="https://github.com/user-attachments/assets/7e3d3fec-ba18-4771-8d5c-b1cb5260f390" />
</p>
<p>
54 On the right click "Rename this PC (advanced). 
<p>
<img <img width="1440" alt="DE_54" src="https://github.com/user-attachments/assets/3fd1df47-ad74-49be-b773-b502253d854e" />
</p>
<p>
56 Under the Computer Name tab click "Change". 
<p>
<img <img width="1440" alt="DE_56" src="https://github.com/user-attachments/assets/435f8e11-4264-4d99-b2f9-383ccd792acc" />
</p>
<p>
57 In Domain box type in "mydomain.com" and click "OK".
<p>
<img <img width="1440" alt="DE_57" src="https://github.com/user-attachments/assets/8e99c250-c3af-4b42-87d6-b20fe5017cf0" />
</p>
<p>
58 Because we set the DNS settings to use dc-1's private IP address its able to locate the domain controller. 
   Now type in the login credentials for the admin we created earlier and click "OK". 
<p>
<img <img width="1440" alt="DE_58" src="https://github.com/user-attachments/assets/b40165a9-f903-413d-a978-723e2aeb6da7" />
</p>
<p>
59 You will see this pop-up welcoming you to mydomain.com. 
   Then click "OK".
<p>
<img <img width="1440" alt="DE_59" src="https://github.com/user-attachments/assets/29951859-4573-4e4b-aff6-8b780fabace3" />
</p>
<p>
60 After this change the computer will need to restart. 
   Click "OK".
<p>
<img <img width="1440" alt="DE_60" src="https://github.com/user-attachments/assets/9474bbc2-daff-4f85-bbf4-3d076af252ff" />
</p>
<p>
61 Close the System Properties. 
<p>
<img <img width="1440" alt="DE_61" src="https://github.com/user-attachments/assets/009feddf-d81f-4c0c-b910-8a9b13cdc20c" />
</p>
<p>
62 Click "Restart Now".
<p>
<img <img width="1256" alt="Screenshot 2025-07-04 at 1 29 40 PM" src="https://github.com/user-attachments/assets/bcc0a938-5524-4c9d-b935-48e48775fe2f" />
</p>
<p>
63 Now we are going to login to the Domain Controller and verify that client-1 is in the ADUC
   Go back to dc-1 and in the search bar at the bottom search for Active Directory Users and Computers". 
   Click the App when it appears. 
<p>
<img <img width="1440" alt="DE_63" src="https://github.com/user-attachments/assets/7189ac0c-64ee-446e-919f-322922b85cf7" />
</p>
<p>
64 Click the drop down arrow for mydomain.com and click the computers folder. 
   As you can see client-1 has been added. 
<p>
<img <img width="1440" alt="DE_64" src="https://github.com/user-attachments/assets/3c1d505a-11e9-444a-b0e4-75e143354e14" />
</p>
<p>
65 If you double click it you can see all the properties of that computer. 
<p>
<img <img width="1440" alt="DE_65" src="https://github.com/user-attachments/assets/e834057b-6d8a-4e6a-b248-0b72e99c495b" />
</p>
<p>
68 Now we are going to create a new organizational unit called clients. 
   Right click mydomain.com
   Click "New"
   Click "Organizational Unit"
<p>
<img <img width="1440" alt="DE_68" src="https://github.com/user-attachments/assets/8e32587e-440e-4cd9-8ebe-88c8f9f70243" />
</p>
<p>
69 Name it _CLIENTS and click "OK".
<p>
<img <img width="1440" alt="DE_69" src="https://github.com/user-attachments/assets/5fe6daa6-389b-4ce7-9967-b2afa7578cef" />
</p>
<p>
70 Now from the computers folder grab client-1 and drop it into the _CLIENTS folder. 
<p>
<img <img width="1440" alt="DE_70" src="https://github.com/user-attachments/assets/11600caf-9ed0-418c-8b12-86054e95f9f4" />
</p>
<p>
71 Click "Yes"
   That was made to make the organization a little bit easier. 
<p>
<img <img width="1440" alt="DE_71" src="https://github.com/user-attachments/assets/78499e0d-5f69-4b5c-a554-34b5f17339c4" />
</p>
<p>
72 Right click mydomain.com and click "Refresh".
<p>
<img <img width="1440" alt="DE_72" src="https://github.com/user-attachments/assets/877d726d-8e37-4ec4-883d-7f01d868c29f" />
</p>
<p>
73 Now we can go down the list and see everything that is there. 
   We have our admin. 
<p>
<img <img width="1440" alt="DE_73" src="https://github.com/user-attachments/assets/73d4de34-26df-40a4-a23d-f8d16c46f68d" />
</p>
<p>
74 There is client-1 
<p>
<img <img width="1440" alt="DE_74" src="https://github.com/user-attachments/assets/7a82bd5a-345b-4370-b5a4-f49b49cd7749" />
</p>
<p>
75 Also our employees. There is nothing in there yet but we will add them shortly. 
  The link to the Repository at the top will take you to the next portion of the tutorial. 
<p>
<img <img width="1440" alt="DE_75" src="https://github.com/user-attachments/assets/02d3c28e-f82c-437c-878f-b3d71c776159" />
</p>
<p>
