# DeployAspCoreOnNginx
Deploy AspCore on Nginx

# Install Nginx on centos

```bash
sudo yum -y update
sudo yum install -y epel-release
sudo yum –y install nginx

sudo systemctl start nginx

sudo systemctl status nginx

sudo systemctl enable nginx
```
# Install Firewall

```bash
sudo yum install firewalld
sudo firewall-cmd --state

sudo systemctl start firewalld
sudo systemctl enable firewalld

firewall-cmd --zone=public --permanent --add-service=http
firewall-cmd --zone=public --permanent --add-service=https

firewall-cmd --reload
```
