## Project 1 ##

### WEB STACK IMPLEMENTATION (LAMP STACK) IN AWS


#### LAMP (Linux, Apache, MySQL, PHP or Python, or Perl)
After successful completion of PBL project 1, you will be able to achieve the following.
Become very confident on the Linux Terminal

Deepen your understanding of Web Stacks and familiarity between the differences between the different Web Technology stacks such as LAMP.

Solid Linux administration skills in Storage management, NFS, troubleshooting, and basic networking

**Step 0** 

Provision an EC2 instance, name it *projectLAMP* 

Allow inbound traffic on port 22 for ssh connectivity

![EC2 Instance](instance-created-pr1.jpg)
EC2 Instance

![](ssh-inboundrule-pr1.jpg)
SSH Inbound Rule

Connect to the EC2 Instance

![](instance-connection.jpg)
Instance connected

Update and Upgrade Ubuntu installation by running

```
sudo apt update -y && sudo apt upgrade -y
```

### STEP 1 — INSTALLING APACHE AND UPDATING THE FIREWALL
Apache HTTP Server is the most widely used web server software. Apache is an open source software available for free. It runs on 67% of all webservers in the world. It is fast, reliable, and secure. It can be highly customized to meet the needs of many different environments by using extensions and modules.

Install Apache using *apt* which is package (software) manager used in Ubuntu and some other Linux istributions.

```
sudo apt install apache2
```

Verify if apache is running with

```
sudo systemctl status apache2
```
If you see a green *active (running)* then you have done everything correctly. 

Use

```
 curl http://localhost:80
or
 curl http://127.0.0.1:80
 ```
 to confirm if our new web server is working correctly. You should some HTLM codes on your terminal as an indication that the Apache web server is working okay.

