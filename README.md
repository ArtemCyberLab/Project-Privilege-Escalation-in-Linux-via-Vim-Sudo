In this project, I demonstrated the process of exploiting a vulnerability in a Linux system to achieve privilege escalation. The vulnerability was due to an improper configuration of permissions, where the user mitch was able to run the vim program with root privileges without being prompted for a password. This configuration flaw allowed me to bypass restrictions and gain full access to the system.

Steps taken to exploit the vulnerability:

Connecting to the remote machine: I connected to the system via SSH using the mitch user login. After entering the password, I successfully logged into the system.

Checking user permissions: After logging in, I used a command to check the available commands that could be run with root privileges. The results showed that the user mitch could run the vim program as root without a password prompt.

Exploiting the vulnerability via Vim: Using the ability to run vim, I leveraged it to execute a shell command with root privileges, which granted me full control over the system.

Flag retrieval: After obtaining root privileges, I navigated to the /root directory and read the root.txt flag, confirming successful privilege escalation and full system access.

Conclusion: The process ended with successful root access, confirmed by the presence of the flag and the completion of all steps. I was able to demonstrate how local configuration vulnerabilities can lead to complete system compromise.

This project illustrates how improper sudo configuration can be exploited for privilege escalation, providing full access to the machine and its data.
