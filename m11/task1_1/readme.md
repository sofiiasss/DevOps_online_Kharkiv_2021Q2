**Docker Task**

1. Installing Docker:
```
sudo apt update
sudo apt install \
apt-transport-https\
ca-certificates\
curl\
gnupg-agent\
software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg| sudo apt-key add –
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release-cs) stable"
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io
```

2. Run our first docker container:
```
sudo docker run hello-world
```

3. Creating our first Dockerfile and container:
```
mkdir dockerfiles - creating directory
cd dockerfiles - change directory to new
touch Dockerfile - create Dockerfile
nano Dockerfile -  edit Dockerfile

Containing of Dockerfile:
RUN apt-get -y update
RUN apt-get -y install apache2
RUN echo 'finally!' > /var/www/html/index.html
CMD ["/usr/sbin/apache2ctl", "-DFOREGROUND"]
EXPOSE 80
```
<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/dockerfile.png" >
<break>

Build:
<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/build_im1.png" >
<break>

Results:
<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/finally.png" >
<break>

4. Creating container with app:
<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/app.png" >
<break>

<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/html.png" >
<break>

Build:
<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/docker_build_cats.png" >
<break>

Run:
<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/docker_run_czts.png" >
<break>

Result:
<break>
<img src="https://github.com/sofiiasss/DevOps_online_Kharkiv_2021Q2/blob/master/m11/task1_1/images/res.png" >
<break>

