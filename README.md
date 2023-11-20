<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com/watch?v=HGywPhfKt4E)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Configuration Steps</h2>

<p>
1. This is a continuation from osTicket - Prerequisites and Installation, available at https://github.com/Gleejr/osticket-prereqs. Once osTicket has been successfully installed, you can proceed with the next steps.
</p>
<p>
<img width="777" alt="Screen Shot 2023-11-17 at 10 20 24 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/5f890a1d-6742-4001-a6d8-6e36984969c1">
</p>

<p>
2. Log in to osTicket by following this link: http://localhost/osTicket/scp/login.php. Use the 'user_admin' account that was created, with the password 'Password1234'. This will take you to the osTicket dashboard.
<p>
<img width="618" alt="Screen Shot 2023-11-17 at 10 25 59 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/0e817fd3-3cca-49f5-b70d-a02fcc2b643e">
<img width="1003" alt="Screen Shot 2023-11-17 at 10 27 54 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/956a2670-10c9-4dab-9e77-68d25fd55909">
</p>

<h3>Configure Roles</h3>
<p>
3. In the admin panel, click on 'Agents,' then select 'Roles,' and click on 'Add a New Role.'
</p>
<p>
<img width="954" alt="Screen Shot 2023-11-17 at 10 37 13 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/0b2d0a2f-7ba6-4934-8624-781f015c5346">
<img width="1009" alt="Screen Shot 2023-11-17 at 10 38 43 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/a31ce1cf-17e4-4195-82ab-8e765993a248">
<img width="1007" alt="Screen Shot 2023-11-17 at 10 41 13 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/3e603dc4-420e-4cae-8f24-d511db93ce43">
</p>

<p>
4. Name this role 'Supreme Admin' and, under permissions, check every box. Click 'Add Role' to finish.
</p>
<p>
<img width="963" alt="Screen Shot 2023-11-17 at 10 47 52 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/a8c54f4a-dafe-45ef-acf4-49bcae6523da">
<img width="954" alt="Screen Shot 2023-11-17 at 10 45 34 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/adc327af-ccf0-4c86-948e-bc51600f11c9">
</p>

<h3>Configure Departments</h3>
<p>
5. In the admin panel, navigate to the 'Agents' tab, click on 'Departments,' and add a new department.
</p>
<p>
<img width="964" alt="Screen Shot 2023-11-17 at 10 53 40 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/d661d400-93a4-46a1-b53f-33091138948a">
<img width="1021" alt="Screen Shot 2023-11-17 at 10 55 16 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/da496a26-3a01-4c14-ad90-f3d173c57101">
</p>

<p>
6. Enter the name 'System Administrators,' leave everything else as default, and click 'Create Department.'
</p>
<p>
<img width="1440" alt="Screen Shot 2023-11-17 at 10 59 38 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/9bd9aff6-fa67-4cda-bd46-8dff9db02cf3">
<img width="622" alt="Screen Shot 2023-11-18 at 1 29 04 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/9f442941-9ed3-47cb-a55d-30fd88aef672">
</p>

<h3>Configure Teams</h3>
<p>
7. In the admin panel, go to the 'Agents' tab, click on 'Teams,' and then select 'Add New Team.'
</p>
<p>
<img width="852" alt="Screen Shot 2023-11-18 at 1 32 22 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/2ac6aad5-d8a2-45a1-81ac-29f78bbc6f8c">
<img width="934" alt="Screen Shot 2023-11-18 at 1 34 54 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/8cbe7cc2-499f-49fc-beb6-bb855ae07f28">
</p>

<p>
8. Enter the name 'Level II Support,' add yourself to the team, and click on 'Create Team.'
</p>
<p>
<img width="890" alt="Screen Shot 2023-11-18 at 1 37 52 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/21c7390b-fd44-4fe6-8caf-93ea2df6b748">
<img width="888" alt="Screen Shot 2023-11-18 at 1 38 31 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/bd822b4a-23d9-4bd9-aa6f-2cac5714344d">
</p>

<h3>Allow anyone to make tickets</h3>
<p>
9. In the admin panel, navigate to 'Settings' and scroll down to 'Users.' Ensure that 'Require registration and login to create tickets' is unchecked. This will allow anyone to create tickets anonymously.
</p>
<p>
<img width="835" alt="Screen Shot 2023-11-18 at 1 44 52 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/c9dbd089-fd63-48b4-be37-ea6d45c5fca2">
<img width="799" alt="Screen Shot 2023-11-18 at 1 47 12 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/c573f74b-ed2b-4ad2-a135-8481ae4410be">
</p>


<h3>Configure Agents</h3>
<p>
9. In the admin panel, go to the 'Agents' tab and click on 'Add New Agent.'
</p>
<p>
<img width="930" alt="Screen Shot 2023-11-18 at 1 51 57 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/770f6bbe-1502-4f3f-896b-67e8ec7e6446">
</p>

<p>
10. Enter the name of the agent (Jane Doe), the email (jane.doe@osticket.com), and the username (jane.doe). Click on 'Set Password.'
</p>
<p>
<img width="917" alt="Screen Shot 2023-11-18 at 1 55 33 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/f8939548-ca9e-4ab4-8703-3f53d2156164">
</p>

<p>
11. Uncheck 'Send the agent a password reset email,' enter a password for this agent, uncheck 'Require password change at next login,' and click on 'Set.'
</p>
<p>
<img width="650" alt="Screen Shot 2023-11-18 at 1 59 51 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/0b2a42cf-469d-4852-95eb-5bfc23dc3895">
</p>

<p>
12. Go to the 'Access' tab, set the department to 'System Administrators' and the role to 'Supreme Admin.' Under extended access, add 'Support' for the department and 'Supreme Admin' for the role.
</p>
<p>
<img width="962" alt="Screen Shot 2023-11-19 at 12 07 55 AM" src="https://github.com/Gleejr/post-install-config/assets/148407820/6b200236-e518-4e29-a7c0-16e226dc2cea">
<img width="964" alt="Screen Shot 2023-11-19 at 4 50 18 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/980d64c0-8efc-42a8-92f7-0210b8e54808">
</p>

<p>
13. Navigate to the 'Teams' tab, assign the agent to 'Level II Support,' and click on 'Create.'
</p>
<p>
<img width="982" alt="Screen Shot 2023-11-19 at 12 12 50 AM" src="https://github.com/Gleejr/post-install-config/assets/148407820/d7bba9bc-9227-4563-83da-810913571bb5">
</p>

<p>
14. Repeat the same steps to create another agent (John Doe/username: john.doe, email: john.doe@osticket.com). Assign this agent to the 'Support' department, grant all access for roles, and set 'Support' for extended access.
</p>
<p>
<img width="962" alt="Screen Shot 2023-11-19 at 12 18 30 AM" src="https://github.com/Gleejr/post-install-config/assets/148407820/e7fcd2c3-9170-4421-8606-0739b5ea8840">
<img width="982" alt="Screen Shot 2023-11-19 at 12 20 30 AM" src="https://github.com/Gleejr/post-install-config/assets/148407820/684b7d69-4322-4f6d-9513-0ab7b5d48407">
</p>



<h3>Configure Users</h3>
<p>
15. In the agent panel, navigate to 'Users' and click on 'Add User.' Enter 'Karen Karen' for the name and the email 'karen@osticket.com.' Click on 'Add User.'
</p>
<p>
<img width="966" alt="Screen Shot 2023-11-19 at 2 20 31 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/3033a20a-3cc3-4857-8708-616e240a957e">
<img width="644" alt="Screen Shot 2023-11-19 at 2 26 20 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/2dbc8038-345c-493b-8958-40fc945f9442">
</p>

<p>
16. Repeat the same steps to create a new user. Enter 'Ken Ken' for the name and the email 'ken@osticket.com.' Click on 'Add User.'
</p>
<p>
<img width="648" alt="Screen Shot 2023-11-19 at 2 28 16 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/c1d6f0c9-4465-4471-84ce-c7824f66a764">
</p>

<h3>Configure SLA</h3>
<p>
17. In the admin panel, navigate to 'Manage' and click on 'SLA.' Then, click on 'Add New SLA Plan.'
</p>
<p>
<img width="969" alt="Screen Shot 2023-11-19 at 2 31 54 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/746788d0-485c-485c-9045-ce51566b4da8">
<img width="963" alt="Screen Shot 2023-11-19 at 2 33 44 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/38ab8695-a344-4dc6-b29b-a30922382836">
</p>

<p>
18. Enter 'SEV-A' for the name, set the grace period to 1 hour, and choose a 24/7 schedule. Click 'Add Plan.'
</p>
<p>
<img width="950" alt="Screen Shot 2023-11-19 at 2 37 47 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/e04d5bc3-7f0f-45b3-a56b-ff97dd62b0ca">
</p>

<p>
19. Enter 'SEV-B' for the name, set the grace period to 4 hours, and choose a 24/7 schedule. Click 'Add Plan.'
</p>
<p>
<img width="956" alt="Screen Shot 2023-11-19 at 2 41 12 PM 1" src="https://github.com/Gleejr/post-install-config/assets/148407820/7c87d5c6-4e30-41cc-9fb7-5e2af1643dcc">
</p>

<p>
20. Enter 'SEV-C' for the name, set the grace period to 8 hours, and choose a schedule of Monday - Friday, 8 am - 5 pm, including US Holidays. Click 'Add Plan.'
</p>
<p>
<img width="963" alt="Screen Shot 2023-11-19 at 3 01 02 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/9a1cd2e9-39bd-4ea5-848a-5bd5a283b3ee">
</p>
<br />

<h3>Configure Help Topics</h3>
<p>
21. In the admin panel, navigate to 'Manage' and click on 'Help Topics.' Then, click on 'Add New Help Topic.'
</p>
<p>
<img width="959" alt="Screen Shot 2023-11-19 at 3 06 54 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/d199a605-df12-4690-9cac-ac018cdbe9dc">
<img width="967" alt="Screen Shot 2023-11-19 at 3 07 46 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/a49607e8-bdc1-4db5-a937-6425b83c2ee2">
</p>

<p>
22. Enter 'Business Critical Outage' as the topic and click 'Add Topic.'"
</p>
<p>
<img width="966" alt="Screen Shot 2023-11-19 at 3 11 28 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/95bf5386-6b3b-43ab-ad53-e469487f694a">
</p>

<p>
23. Enter 'Personal Computer Issues' as the topic and click 'Add Topic.'
</p>
<p>
<img width="961" alt="Screen Shot 2023-11-19 at 3 14 16 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/d80db4a2-4ff7-4556-ac1e-354a43d7f8c6">
</p>

<p>
24. Enter 'Equipment Request' as the topic and click 'Add Topic.'
</p>
<p>
<img width="969" alt="Screen Shot 2023-11-19 at 3 16 12 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/814d1f86-9311-47a0-8729-c014dddcaeb3">
</p>

<p>
25. Enter 'Password Reset' as the topic and click 'Add Topic.'
</p>
<p>
<img width="963" alt="Screen Shot 2023-11-19 at 3 17 29 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/7496f30a-0dff-4b16-9cc8-83b8037e3788">
</p>






<br />
