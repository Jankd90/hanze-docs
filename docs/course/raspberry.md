# Getting started

install rasbien on a sd card >>> todo

## Commands

* `ifconfig` - list networking info on pi.

<div class="admonition warning">
<p class="admonition-title">Do try this at home</p>
<p>...</p>
</div>

    
## Configure ssh
  
run:
``` Bash
ifconfig
```
and find the inet ip > e.g. 192.168.178.26
``` Bash
sudo raspi-config
```
go to 5 (Interfacing Options),
then to p2, ssh and enable. 

on your computer open a terminal:

``` Bash
ssh pi@ 192.168.178.26
```

pasword is raspberry by default.


