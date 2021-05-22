**CI/CD**
1. Configuring and installing Jenkins on our host-machine:
```
wget -q   -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo nano /etc/apt/sources.list
deb https://pkg.jenkins.io/debian-stable binary/ (add this text)
sudo apt-get update
java -version
sudo apt-get install openjdk-8-jdk
sudo apt-get install jenkins
service jenkins status
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```

2. Going to **http://vm-ip:8080**

3. Configuring Jenkins:
- installing suggesting plugins;
- adding user;
- creating password.

4. Creating simple job:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m8/images/item.jpg">
<br>
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m8/images/shell.jpg">
<br>

5. Installing Apache2 on the second VM:
```
sudo apt update
sudo apt install apache2
```

6. Going to vm2-ip to check state of Apache2 - we must see default Apache2 page.

7. Creating ssh keys:
```
ssh-keygen
```

8. Go to vm2 by SSH.

9. Copy id of vm2.

10. Go to Jenkins to execute shell and write:
```
scp -v -o StrictHostKeyChecking=no index.html username@vm2-ip:/var/www/html (default apache2's directory)
```

11. Result:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m8/images/scp.jpg" >
<br>

12. Install **Publish over SSH** plugin.

13.Publish private key, vm2-ip, username, home directory to ssh-configure.

14. Result:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m8/images/overssh.jpg" >
<br>