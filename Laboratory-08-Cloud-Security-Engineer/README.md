# Laboratory 08: Cloud Security Engineer

## Mission Overview

This laboratory activity focuses on securing an Ubuntu server using the UFW host-based firewall. I deployed an Nginx web application and configured firewall rules to control incoming and outgoing network traffic.

## Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a virtual machine.
- Apply a default-deny incoming firewall policy.
- Allow SSH and the web application port.
- Verify firewall rules and test the web application.

## Commands Executed

```bash
docker run -d -p 8080:80 --name secure-web-app nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

I learned how to deploy an Nginx container, configure UFW firewall rules, and check the firewall status. I also learned why SSH access should be allowed before enabling the firewall and why limiting open ports helps reduce security risks.
