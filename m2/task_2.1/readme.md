**Part 1**
1. The most popular hypervisors are Hyper-V, VMware, Oracle VM, etc.
2. **Hyper-V**. It is already mounted to your computer and you don't need any license or activation key.
**VMware**. It is suitable for great developers; you need license.
**Oracle VM**. It is most popular within students that have no expirience; it is free.

**Part 2**
Oracle VM has friendly and intuitive interface. Creating a VM doesn't take much time; cloning it to.
Commands (in this case were buttons), that we have used to explore this tool:
''' 
button start - start a VM
button stop - stop VM and requires to choose one way in which VM will be stopped (save state, turn off or and send a signal to turn off it)
button reboot - restart a VM
button save state - saves state of VM
'''
Snapshots are used to save states and if it needs to return to any moment, it could be reestablished from snaps.
![]
(C:\Users\Sofiya\DevOps_online_Kharkiv_2021Q2\m2\task_2.1\images\snap.jpg)

The next steps were exporting, importing VM, configuring USB connection and creating folders to exchange files.
Table of connections.
![]
(C:\Users\Sofiya\DevOps_online_Kharkiv_2021Q2\m2\task_2.1\images\table.jpg)

Сommands used in the command line correspond to buttons on the interface.

**Part 3**
Commands that were used:
'''
mkdir 
vagrant init
vagrant up
vagrant halt
vagrant destroy
vagrant package
vagrant box add
'''
Download enviroment, create folder and initialize the enviroment.
Then ran vagrant and booted a VM.
Connected to VM with Putty.
![]
(C:\Users\Sofiya\DevOps_online_Kharkiv_2021Q2\m2\task_2.1\images\date.jpg)

Then stopped a VM and destoyed it.
![]
(C:\Users\Sofiya\DevOps_online_Kharkiv_2021Q2\m2\task_2.1\images\destroy.jpg)

Creating box:
![]
(C:\Users\Sofiya\DevOps_online_Kharkiv_2021Q2\m2\task_2.1\images\box.jpg)

List of boxes:
![]
(C:\Users\Sofiya\DevOps_online_Kharkiv_2021Q2\m2\task_2.1\images\box2.jpg)