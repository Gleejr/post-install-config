<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

<p>
1. This is a continuation from osTicket - Prerequisites and Installation https://github.com/Gleejr/osticket-prereqs once osTicket has been successfully installed. 
</p>
<p>
<img width="777" alt="Screen Shot 2023-11-17 at 10 20 24 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/5f890a1d-6742-4001-a6d8-6e36984969c1">
</p>

<p>
2. Login to osTicket using this "link http://localhost/osTicket/scp/login.php". Use the user_admin account that was created with the password1234. This will bring you inside osTicket.
<p>
<img width="618" alt="Screen Shot 2023-11-17 at 10 25 59 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/0e817fd3-3cca-49f5-b70d-a02fcc2b643e">
<img width="1003" alt="Screen Shot 2023-11-17 at 10 27 54 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/956a2670-10c9-4dab-9e77-68d25fd55909">
</p>

<h3>Configure Roles</h3>
<p>
3. In the admin panel click on agents, click on roles. and select add a new role.
</p>
<p>
<img width="954" alt="Screen Shot 2023-11-17 at 10 37 13 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/0b2d0a2f-7ba6-4934-8624-781f015c5346">
<img width="1009" alt="Screen Shot 2023-11-17 at 10 38 43 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/a31ce1cf-17e4-4195-82ab-8e765993a248">
<img width="1007" alt="Screen Shot 2023-11-17 at 10 41 13 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/3e603dc4-420e-4cae-8f24-d511db93ce43">
</p>

<p>
4. Name this role "Supreme Admin" and under permissions check every box. Click add role to finish.
</p>
<p>
<img width="963" alt="Screen Shot 2023-11-17 at 10 47 52 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/a8c54f4a-dafe-45ef-acf4-49bcae6523da">
<img width="954" alt="Screen Shot 2023-11-17 at 10 45 34 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/adc327af-ccf0-4c86-948e-bc51600f11c9">
</p>

<h3>Configure Departments</h3>
<p>
5. In the admin panel, in the agents tab click departments and add a new department.
</p>
<p>
<img width="964" alt="Screen Shot 2023-11-17 at 10 53 40 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/d661d400-93a4-46a1-b53f-33091138948a">
<img width="1021" alt="Screen Shot 2023-11-17 at 10 55 16 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/da496a26-3a01-4c14-ad90-f3d173c57101">
</p>

<p>
6. Input the name "System Administrators", leave everything else on default, and click "create Department".
</p>
<p>
<img width="1440" alt="Screen Shot 2023-11-17 at 10 59 38 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/9bd9aff6-fa67-4cda-bd46-8dff9db02cf3">
<img width="622" alt="Screen Shot 2023-11-18 at 1 29 04 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/9f442941-9ed3-47cb-a55d-30fd88aef672">
</p>

<h3>Configure Teams</h3>
<p>
7. In the admin panel, in the agents tab click on teams and click on add new team.
</p>
<p>
<img width="852" alt="Screen Shot 2023-11-18 at 1 32 22 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/2ac6aad5-d8a2-45a1-81ac-29f78bbc6f8c">
<img width="934" alt="Screen Shot 2023-11-18 at 1 34 54 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/8cbe7cc2-499f-49fc-beb6-bb855ae07f28">
</p>

<p>
8. Input the name "Level II Support", add yourself to the team, and click on "create team".
</p>
<p>
<img width="890" alt="Screen Shot 2023-11-18 at 1 37 52 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/21c7390b-fd44-4fe6-8caf-93ea2df6b748">
<img width="888" alt="Screen Shot 2023-11-18 at 1 38 31 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/bd822b4a-23d9-4bd9-aa6f-2cac5714344d">
</p>

<h3>Allow anyone to make tickets</h3>
<p>
9. In the admin panel, go to setting and scroll down to users. Make sure "Require registration and login to create tickets" is unchecked. This will allow anyone to create tickets anonymously.
</p>
<p>
<img width="835" alt="Screen Shot 2023-11-18 at 1 44 52 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/c9dbd089-fd63-48b4-be37-ea6d45c5fca2">
<img width="799" alt="Screen Shot 2023-11-18 at 1 47 12 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/c573f74b-ed2b-4ad2-a135-8481ae4410be">
</p>


<h3>Configure Agents</h3>
<p>
9. In the admin panel, in the agents tab click on add new agent. 
</p>
<p>
<img width="930" alt="Screen Shot 2023-11-18 at 1 51 57 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/770f6bbe-1502-4f3f-896b-67e8ec7e6446">
</p>

<p>
10. Enter the name of the agent (Jane Doe), the email (jane.doe@osticket.com), and the username (jane.doe). Click on set password.
</p>
<p>
<img width="917" alt="Screen Shot 2023-11-18 at 1 55 33 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/f8939548-ca9e-4ab4-8703-3f53d2156164">
</p>

<p>
11. Uncheck "Send the agent a password reset email", Enter a password for this agent, uncheck "Require password change at next login", and click on set. 
</p>
<p>
<img width="650" alt="Screen Shot 2023-11-18 at 1 59 51 PM" src="https://github.com/Gleejr/post-install-config/assets/148407820/0b2a42cf-469d-4852-95eb-5bfc23dc3895">
</p>


<br />



<br />
