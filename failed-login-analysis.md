# Failed Login Analysis 
## Assignment 1: Failed Login Attack
- What is a failed login attack: An attempt to log in with incorrect credentials, which may indicate brute-force or credential-stuffing activity.
- Systems commonly targeted: Servers, endpoints, cloud services.
- Logs to check: 
     - Windows: Security Event Logs (Event ID 4625)
     - Linux: /var/log/auth.log
- What makes it suspicious vs normal:
     - Suspicious: multiple failures, unusual IPs, invalid usernames
     - Normal: occasional mistyped passwords
- First response as a SOC analyst
     - Identify source IP
     - Check if login eventually succeeded
     - Assess scope and take containment actions

## Assignment 2: Succesful Login After Failures
- Why is this more dangerous: It is more dangerous because it may indicate that an attacker has succesfully guessed or obtained valid credentials
- WHat questions would I ask first: As a SOC analyst, my first question would be to identify the affected account & system, assess the account's privilege level and determine the scope of impact before taking containment actions.
- My first response:
     - Validate if alert is real
     - Assess scope
     - Contain the threat if necessary
