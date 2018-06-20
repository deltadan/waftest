# Web App used to Test Firewalls
This script extention can be used with an Azure Ubuntu VM to build a lab for testing firewalls

**Damn Vulnerable Web Application (DVWA)**

This script will install and configure the DWVA on your Ubuntu VM. Damn Vulnerable Web App (DVWA) is a PHP/MySQL web application that is damn vulnerable. Its main goals are to be an aid for security professionals to test their skills and tools in a legal environment, help web developers better understand the processes of securing web applications and aid teachers/students to teach/learn web application security in a class room environment.

![img](https://github.com/deltadan/waftest/blob/master/media/dvwa.png)

"DVWA application provides attacks to test your WAF")

**Creds**
1. User: admin
1. Password: password

**Install**
1. Clone repo locally
1. Deploy an Ubuntu VM to Azure with a Public IP Address
1. Open a NSG with Port 80 / Allow / TCP
![img](https://github.com/deltadan/waftest/blob/master/media/nsg.png)
1. During provisioning add the Linux Custom script extention and configure to run the waftest.sh
![img](https://github.com/deltadan/waftest/blob/master/media/script.png) "run linux script")
1. After the VM provisions, browse to the Public IP Address /dvwa
1. Publish the VM behind a firewall to test the firewall and then run the attacks

