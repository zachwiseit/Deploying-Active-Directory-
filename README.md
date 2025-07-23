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
1 If you aren't already Remote desktop into dc-1 in the Windows App. 
  (I would recmoned Remoting into both dc-1 and client-1) 
  To help tell which computer is which the Windows ten computer will have the windows shopping app on the task bar. 
  The Windows server will not. 
<p>
<p>
<img <img width="1440" alt="DE_1" src="https://github.com/user-attachments/assets/6aff293b-6db8-4558-b8f8-74db3ec3999e" />
</p>
<p>
3 In dc-1 (windows server) right click start and go to Server Manager. 
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
15 CLick "Install"
<p>
<img <img width="1440" alt="DE_15" src="https://github.com/user-attachments/assets/ec8bb96d-d856-4f63-85c9-c25405a60be9" />
</p>
<p>
16 After the configure installation has installed click "Close".
<p>
<img <img width="1440" alt="DE_16" src="https://github.com/user-attachments/assets/e7d987e0-26a1-4e34-bb0b-0ac6f69f742c" />
</p>
<p>
17
<p>
<img <img width="1440" alt="DE_17" src="https://github.com/user-attachments/assets/58389dc1-bfc2-4a25-ad0b-48e2e9bb9561" />
</p>
<p>
18
<p>
<img <img width="1440" alt="DE_18" src="https://github.com/user-attachments/assets/ba978684-b496-476c-adbe-41c925b95398" />
</p>
<p>
19
<p>
<img <img width="1440" alt="DE_19" src="https://github.com/user-attachments/assets/3bf3d35e-4709-465c-ae69-05294a2b318b" />
</p>
<p>
20
<p>
<img <img width="1440" alt="DE_20" src="https://github.com/user-attachments/assets/341d1b30-1d67-4ffe-bc01-9adf6cf2e394" />
</p>
<p>
21
<p>
<img <img width="1440" alt="DE_21" src="https://github.com/user-attachments/assets/333b689f-0d3d-4e4f-b732-0f9e1795d2b2" />
</p>
<p>
22
<p>
<img <img width="1440" alt="DE_22" src="https://github.com/user-attachments/assets/0a72d999-527e-4ef9-adff-2d619d6938a6" />
</p>
<p>
23
<p>
<img <img width="1440" alt="DE_23" src="https://github.com/user-attachments/assets/cdb7086a-f0a0-419c-9276-398bb2898997" />
</p>
<p>
24
<p>
<img <img width="1440" alt="DE_24" src="https://github.com/user-attachments/assets/7bcacdf4-db13-450c-91ad-37ee69a34677" />
</p>
<p>
25
<p>
<img <img width="1440" alt="DE_25" src="https://github.com/user-attachments/assets/a5e7cfad-ba69-46b5-9165-090bfe1a9a8b" />
</p>
<p>
26
<p>
<img <img width="1440" alt="DE_26" src="https://github.com/user-attachments/assets/2326b4f8-35f1-44f3-b7b5-1d6798a211e4" />
</p>
<p>
27
<p>
<img <img width="1440" alt="DE_27" src="https://github.com/user-attachments/assets/13dd16ac-0209-44fe-b336-03ba78460756" />
</p>
<p>
28
<p>
<img <img width="1440" alt="DE_28" src="https://github.com/user-attachments/assets/e3b611e9-5b91-4dd8-b515-7f3016d6a894" />
</p>
<p>
29
<p>
<img <img width="1440" alt="DE_29" src="https://github.com/user-attachments/assets/28872c1a-b610-423d-a0c3-f78b82c905db" />
</p>
<p>
30
<p>
<img <img width="1440" alt="DE_30" src="https://github.com/user-attachments/assets/86378893-6e3e-4644-a4a9-c0c396fe26cc" />
</p>
<p>
31
<p>
<img <img width="1440" alt="DE_31" src="https://github.com/user-attachments/assets/177c848e-99c9-4b07-81dc-36593a59ab2c" />
</p>
<p>
32
<p>
<img <img width="1440" alt="DE_32" src="https://github.com/user-attachments/assets/004b4393-b745-48f1-8005-b29aa31ca60b" />
</p>
<p>
33
<p>
<img <img width="1440" alt="DE_33" src="https://github.com/user-attachments/assets/1e285941-3353-47d0-b2e2-e4046d066ab1" />
</p>
<p>
34
<p>
<img <img width="1440" alt="DE_34" src="https://github.com/user-attachments/assets/a3ec331a-8c1b-41d5-817f-c07e707b8ee2" />
</p>
<p>
35
<p>
<img <img width="1440" alt="DE_35" src="https://github.com/user-attachments/assets/7ee8f96a-cd96-4009-a0d4-b26b8f199438" />
</p>
<p>
36
<p>
<img <img width="1440" alt="DE_36" src="https://github.com/user-attachments/assets/d09d4060-0c79-4646-8032-190caa5adf6b" />
</p>
<p>
37
<p>
<img <img width="1440" alt="DE_37" src="https://github.com/user-attachments/assets/12074c81-47f0-4435-a8a6-bbeb7779845a" />
</p>
<p>
38
<p>
<img <img width="1440" alt="DE_38" src="https://github.com/user-attachments/assets/4646df5c-d698-4405-ab12-bf4d55d3e7a8" />
</p>
<p>
39
<p>
<img <img width="1440" alt="DE_39" src="https://github.com/user-attachments/assets/aa117a28-0abf-4bad-9959-a91d751db5a3" />
</p>
<p>
40
<p>
<img <img width="1440" alt="DE_40" src="https://github.com/user-attachments/assets/b891d082-a9a1-42c5-bcc9-87ac382fe8ad" />
</p>
<p>
41
<p>
<img <img width="1440" alt="DE_41" src="https://github.com/user-attachments/assets/08eb4df0-8280-43dc-b487-f987382e7d7e" />
</p>
<p>
42
<p>
<img <img width="1440" alt="DE_42" src="https://github.com/user-attachments/assets/c1644c54-dd4e-482e-859b-2cb12d3bfea1" />
</p>
<p>
43
<p>
<img <img width="1440" alt="DE_43" src="https://github.com/user-attachments/assets/3bfe27f5-a28d-4994-b473-488524a1eae6" />
</p>
<p>
44
<p>
<img <img width="1440" alt="DE_44" src="https://github.com/user-attachments/assets/a26102b3-1c11-40c0-b459-713844bdbeae" />
</p>
<p>
45
<p>
<img <img width="1440" alt="DE_45" src="https://github.com/user-attachments/assets/2927796c-a273-4b6e-802b-6483f6736465" />
</p>
<p>
46
<p>
<img <img width="1440" alt="DE_46" src="https://github.com/user-attachments/assets/5923b5a8-d592-4de2-b8a4-f10ac079e781" />
</p>
<p>
47
<p>
<img <img width="1440" alt="DE_47" src="https://github.com/user-attachments/assets/0b8ca342-d5ea-4f92-88a5-71f62e02486d" />
</p>
<p>
48
<p>
<img <img width="1440" alt="DE_48" src="https://github.com/user-attachments/assets/13681512-5001-4612-bcf4-db66388f3de9" />
</p>
<p>
49
<p>
<img <img width="1440" alt="DE_49" src="https://github.com/user-attachments/assets/d9ab7105-b2b0-4ce7-94e2-a90eeb9c9352" />
</p>
<p>
50
<p>
<img <img width="1440" alt="DE_50" src="https://github.com/user-attachments/assets/acaba768-0fa1-482a-bb79-f81259e2fc4f" />
</p>
<p>
51
<p>
<img <img width="1440" alt="DE_51" src="https://github.com/user-attachments/assets/c0bdea20-f650-4fd4-bd90-0faefee2eea1" />
</p>
<p>
52
<p>
<img <img width="1257" alt="Screenshot 2025-07-04 at 1 15 55 PM" src="https://github.com/user-attachments/assets/755f1c05-2a07-44a9-8686-49390d8d0914" />
<p>
53
<p>
<img <img width="1268" alt="Screenshot 2025-07-04 at 1 19 18 PM" src="https://github.com/user-attachments/assets/7e3d3fec-ba18-4771-8d5c-b1cb5260f390" />
</p>
<p>
54
<p>
<img <img width="1440" alt="DE_54" src="https://github.com/user-attachments/assets/3fd1df47-ad74-49be-b773-b502253d854e" />
</p>
<p>
55
<p>
<img <img width="1440" alt="DE_55" src="https://github.com/user-attachments/assets/7757853e-9794-430a-adac-cdeb72684c9a" />
</p>
<p>
56
<p>
<img <img width="1440" alt="DE_56" src="https://github.com/user-attachments/assets/435f8e11-4264-4d99-b2f9-383ccd792acc" />
</p>
<p>
57
<p>
<img <img width="1440" alt="DE_57" src="https://github.com/user-attachments/assets/8e99c250-c3af-4b42-87d6-b20fe5017cf0" />
</p>
<p>
58
<p>
<img <img width="1440" alt="DE_58" src="https://github.com/user-attachments/assets/b40165a9-f903-413d-a978-723e2aeb6da7" />
</p>
<p>
59
<p>
<img <img width="1440" alt="DE_59" src="https://github.com/user-attachments/assets/29951859-4573-4e4b-aff6-8b780fabace3" />
</p>
<p>
60
<p>
<img <img width="1440" alt="DE_60" src="https://github.com/user-attachments/assets/9474bbc2-daff-4f85-bbf4-3d076af252ff" />
</p>
<p>
61
<p>
<img <img width="1440" alt="DE_61" src="https://github.com/user-attachments/assets/009feddf-d81f-4c0c-b910-8a9b13cdc20c" />
</p>
<p>
62
<p>
<img <img width="1256" alt="Screenshot 2025-07-04 at 1 29 40 PM" src="https://github.com/user-attachments/assets/bcc0a938-5524-4c9d-b935-48e48775fe2f" />
</p>
<p>
63
<p>
<img <img width="1440" alt="DE_63" src="https://github.com/user-attachments/assets/7189ac0c-64ee-446e-919f-322922b85cf7" />
</p>
<p>
64
<p>
<img <img width="1440" alt="DE_64" src="https://github.com/user-attachments/assets/3c1d505a-11e9-444a-b0e4-75e143354e14" />
</p>
<p>
65
<p>
<img <img width="1440" alt="DE_65" src="https://github.com/user-attachments/assets/e834057b-6d8a-4e6a-b248-0b72e99c495b" />
</p>
<p>
66
<p>
<img <img width="1440" alt="DE_66" src="https://github.com/user-attachments/assets/4bb940d8-375a-4bee-9c17-50a996daf556" />
</p>
<p>
67
<p>
<img <img width="1440" alt="DE_67" src="https://github.com/user-attachments/assets/e0b77191-f00c-4b9d-aa79-f4903633b527" />
</p>
<p>
68
<p>
<img <img width="1440" alt="DE_68" src="https://github.com/user-attachments/assets/8e32587e-440e-4cd9-8ebe-88c8f9f70243" />
</p>
<p>
69
<p>
<img <img width="1440" alt="DE_69" src="https://github.com/user-attachments/assets/5fe6daa6-389b-4ce7-9967-b2afa7578cef" />
</p>
<p>
70
<p>
<img <img width="1440" alt="DE_70" src="https://github.com/user-attachments/assets/11600caf-9ed0-418c-8b12-86054e95f9f4" />
</p>
<p>
71
<p>
<img <img width="1440" alt="DE_71" src="https://github.com/user-attachments/assets/78499e0d-5f69-4b5c-a554-34b5f17339c4" />
</p>
<p>
72
<p>
<img <img width="1440" alt="DE_72" src="https://github.com/user-attachments/assets/877d726d-8e37-4ec4-883d-7f01d868c29f" />
</p>
<p>
73
<p>
<img <img width="1440" alt="DE_73" src="https://github.com/user-attachments/assets/73d4de34-26df-40a4-a23d-f8d16c46f68d" />
</p>
<p>
74
<p>
<img <img width="1440" alt="DE_74" src="https://github.com/user-attachments/assets/7a82bd5a-345b-4370-b5a4-f49b49cd7749" />
</p>
<p>
75
<p>
<img <img width="1440" alt="DE_75" src="https://github.com/user-attachments/assets/02d3c28e-f82c-437c-878f-b3d71c776159" />
</p>
<p>
