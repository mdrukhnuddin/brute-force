Project Name: Brute-Force Attacks – Practical Security Analysis
Organization: Inlighn Tech

Project Overview

I worked on simulating brute-force attacks on vulnerable web applications using Burp Suite Intruder and Hydra. The goal was to understand how attackers exploit weak authentication and to learn mitigation strategies.

Detailed Work Done
1. Setup and Environment

Installed and configured bWAPP/DVWA on a local machine.

Set up Burp Suite proxy to intercept login requests.

Prepared username & password dictionaries for testing.

Configured Hydra and validated target form fields & failure messages.

2. Brute-Force Using Burp Suite

Intercepted login requests with incorrect credentials.

Sent request to Intruder and used Cluster Bomb attack type.

Configured payload positions for username & password fields.

Loaded custom wordlists and executed the attack.

Analyzed status codes and response lengths to detect successful credentials.

Documented the entire process with screenshots.

3. Brute-Force Using Hydra

Identified form action URL (login.php) and input names.

Created Hydra command to automate brute-forcing:
hydra -l admin -P passwords.txt <ip> http-post-form "/bwapp/login.php:login=^USER^&password=^PASS^:Invalid"

Executed attack and monitored output.

Successfully discovered valid password using Hydra.

Recorded results and interpreted server responses.

4. Report & Documentation Work

Created a structured project report with explanations and screenshots.

Added Hydra command syntax variations for different services (SSH, HTTP, FTP).

Prepared mitigation checklist for securing login systems.

Submitted deliverables as required by Inlighn Tech.

Skills Gained

Web application security

Authentication bypass techniques

Practical Burp Suite usage

Hydra automation

HTTP request analysis

Vulnerability assessment

Cyberattack prevention strategies
