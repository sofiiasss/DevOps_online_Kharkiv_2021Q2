**Task 7.1/Bash scripting**
<br>

**Script A**
<br>
```
#!/bin/bash
if [[ $1 = "--all" ]]
then
	cat /etc/hosts
elif [[ $1 = "--target" ]]
	cat /etc/services | grep /tcp
else
	echo Argument --all displays host list.
	echo Argument --target displays TCP ports list.
fi
```
<br>

Option **--all** and **--target** result
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m7/task7.1/images/all.png">
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m7/task7.1/images/target.png">
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m7/task7.1/images/else.png">
<br>

**Script B**
```
#!/bin/bash

awk '{print $11}' $1 | sort | uniq -c | sort -gr  > $2 
{
read line3
} < $2

awk '{print $1}' $1 | sort | uniq -c | sort -gr > $2
{
read line1
} < $2

awk '{print $7}' $1 | sort | uniq -c | sort -gr > $2
{
read line2
} < $2

awk '{print $4}' $1 | sort | uniq -c | sort -gr  > $2 
{
read line4
} < $2

echo $line1 > $2
echo ' ' >> $2
echo $line2 >> $2
echo ' ' >> $2

awk '{print $1}' $1 | sort | uniq -c | sort -gr >> $2

echo ' ' >> $2
echo $line3 >> $2
echo ' ' >> $2
echo $line4 >> $2
echo ' ' >> $2
```
<br>

Results:
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m7/task7.1/images/cat1.png">
<br>
<img src="https://github.com/HighLandner/DevOps_online_Kharkiv_2021Q1/blob/master/m7/task7.1/images/cat2.png">
<br>