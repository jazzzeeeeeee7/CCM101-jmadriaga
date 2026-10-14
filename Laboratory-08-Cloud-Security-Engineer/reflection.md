# Laboratory 08 Reflection: Cloud Security Engineer

This laboratory helped me understand why server security is important in cloud computing. I learned that a firewall adds protection to a server by controlling which network connections are allowed, even if another layer of network security has been breached.

Managing open ports helps reduce the attack surface because fewer exposed services mean fewer possible entry points for attackers. Each open port should have a clear purpose, and unnecessary ports should remain closed. For example, exposing a database port such as 3306 to the public internet can be dangerous because attackers may attempt unauthorized access, exploit vulnerabilities, or guess weak credentials.

Before this activity, I mostly thought about making applications work correctly. After configuring UFW, I realized that deploying an application is not enough; I must also consider who can connect to it and which ports are accessible. I also learned why allowing SSH before enabling the firewall is important to avoid losing remote administrative access.

Adding this mission to my GitHub portfolio makes my cloud computing activities more complete. My previous missions covered areas such as cloud infrastructure, containers, deployment, and operations, while this activity introduced practical firewall configuration and security concepts. Together, these projects help demonstrate my progress in learning cloud technologies.

Overall, this mission taught me to consider security during deployment instead of treating it as a separate task. In future IT projects, I want to continue learning how to configure secure services, review network access, and apply security rules carefully.
