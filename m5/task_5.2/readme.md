**Task 5.2**
<br>
```
**/etc/passwd** directory contains brief info about users: their passwords (password overviews only in **/etc/shadow** with sudo), 
**UID** - user unique identifier, 
**GID** - group unique identifier that user participate, their directory location. 
```
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m5/task5.2/images/passwd.png">
<br>

```
**/etc/group** directory contains only users` group info.
```
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m5/task5.2/images/group.png">
<br>

```
-g parameter shows only the effective GID, -G parameter shows all GIDs
```
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m5/task5.2/images/id.png">
<br>

```
**useradd** adds new user. 
**-c** parameter leaves UID comment, 
**-d** defines user directory, 
**-g** defines user group, 
**-e** - expire date.
```
<br>
**userdel** deletes user account.
<br>
**sudo deluser username** with --remove-all-files parameter deletes user with all his data.
<br>
**usermod** changes user options. -l parameter changes user`s name, -g adds user to certain group, -L locks user account, -U unlocks user.
<br>
**skell_dir** is a directory that contains copy files to recently created directory.
<br>

**Extended directory info**. 
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m5/task5.2/images/la.png">
<br>

**chmod 755** to file provides full-access to user, just read-executable to group and others. Sticky bit is absent. Stickey bit is a bit that prevents user to delete directory, command interpretation - chmod 1755 filename, where 1 is a stikey bit pointer.
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m5/task5.2/images/rwx.png"> 
<br>






 
