**Task 6.2**
<br>

DHCP using ISCDHCP.
<br>
Configurating **/etc/dhcp/dhcp.conf** at clients` workstations.
<br>
```
auto enp0s3
iface enp0s3 inet dhcp
```
<br>

Configurating at server`s workstation.
<br>
```
default-lease-time 7200;
max-lease-time 43200;

subnet 192.168.0.0 netmask 255.255.255.0 {
 range 192.168.0.100 192.168.0.200;
 option routers 192.168.0.1;
 option domain-name-servers 192.168.0.1;
}
```
<br>
where default-lease-time is server rent time if client didn`t ask for another. 
Range - available address range, option router and option DNS - is server`s address.
<br>

**DHCP** using **dnsmasq**.
<br>

Configurating at three clients` workstations.
<br>
```
auto enp0s3
iface enp0s3 inet dhcp
```
<br>

Configurating at server`s workstation.
<br>
```
auto enp0s3
iface enp0s3 inet static
address 192.168.1.1
network 192.168.1.0
netmask 255.255.255.0
broadcast 192.168.1.255
```
<br>

Configurating /etc/dnsmasq.conf. Searching for **dhcp-range** and changing it.
<br>
```
dhcp-range=192.168.1.5,192.168.1.10,12h
```
<br>
that will allow to generate five ip addresses. Two in advance.
<br>


