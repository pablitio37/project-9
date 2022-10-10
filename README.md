# project-9
INSTALL AND CONFIGURE JENKINS SERVER

installation of the jenkins server and checking the status to see that it is running


![Capture1](https://user-images.githubusercontent.com/108102087/192898378-bd34e9fc-886b-432a-880e-66339d302f12.PNG)

From your browser access http://<Jenkins-Server-Public-IP-Address-or-Public-DNS-Name>:8080

I got the prompted to provide a default admin password

![Capture2](https://user-images.githubusercontent.com/108102087/192898744-476fda68-a3a1-420e-963c-3efa42025b3d.PNG)

After appyling the jenkins password, i was logged in as seen below

![Capture3](https://user-images.githubusercontent.com/108102087/192899317-ba087a37-88b3-44f2-8f1a-8bddfa7a425c.PNG)
  
  
The installation is completed!
  
![Capture4](https://user-images.githubusercontent.com/108102087/192900176-3ade0df3-a9f2-4a7b-b241-9c835ca7739f.PNG)
  
## Step 2 – Configure Jenkins to retrieve source codes from GitHub using Webhooks

It took me a while before i was able to set up my webhook and to configure Jenkins to retrieve source codes from Github using Webhook

1.The first issue was when i pasted my git reposttory, i got the error "failed to connect to repository error performing git command" i previously use Mobaxterm which whenever i log in into it using my public IP address will always get this phrase "/usr/bin/xauth:  file /home/ubuntu/.Xauthority does not exist" but i will always ignore the statement since i am logged in anyway. But from the Global tool configuration part of my Jenkins, the git session will also have the error indication the path "usr/bin not found". havinf realised these, i decided to use Powershell instead of Mobaxterm and it worked.

2. another issue faced was after i configured my jenkins, the console output indicate a failed process until i changed the branch to build to main from master.

![project_9](https://user-images.githubusercontent.com/108102087/194921697-ea301aa8-3620-4cb6-82c8-6a2614e1354f.PNG)

"Configure" your job/project and add these two configurations

checking the changes made, A new build was created

![text 2](https://user-images.githubusercontent.com/108102087/194925075-2de590ab-d2c0-4190-aa30-a214398cc1bc.PNG)

