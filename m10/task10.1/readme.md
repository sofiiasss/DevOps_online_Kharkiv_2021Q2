**Ansible**

1. Launch AWS instances.
2. Connect to them.
3. Install Python and Ansible on master.
```
sudo apt-add-repository ppa:ansible/ansible
sudo apt update
sudo apt install ansible
ansible--version
sudoapt install python-pip
```
4. Add *.pem-keys to ssh-directory.
5. Create file hosts.txt and add ansible user.
6. Check connection:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/host.png" >
<br>
7. Modify inventory in ansible config. Check connection again:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/host2.png" >
<br>
8. Some commands:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/inventory.png" >
<br>
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/shell.png" >
<br>
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/changing.png" >
<br>
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/change2.png" >
<br>
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/rm.png" >
<br>
 
**Playbooks**
The first one:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/pb1.png" >
<br>

The second one:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/pb2.png" >
<br>

The third one:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/pb3.png" >
<br>

Results:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/res1.png" >
<br>
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/res2.png" >
<br>

The fourth one:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/pb4.png" >
<br>

The fifth one:
<br>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m10/task10.1/images/pb5.png" >
<br>