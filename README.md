# Ethical-Hacking_Task-4
Just a internship Task.
# Task 4: Setup and Use a Firewall on Windows/Linux

## Objective

Configure and test basic firewall rules to allow or block traffic.

## Tools

-   Windows Firewall\
-   UFW (Uncomplicated Firewall) on Linux

## Steps

1.  **Open firewall configuration tool**
    -   Windows: Control Panel → System and Security → Windows Defender
        Firewall\
    -   Linux: Use terminal with UFW commands
2.  **List current firewall rules**
    -   Windows: View inbound/outbound rules in the firewall GUI\
    -   Linux: `sudo ufw status verbose`
3.  **Block inbound traffic on port 23 (Telnet)**
    -   Windows: Add new inbound rule in Firewall GUI\
    -   Linux: `sudo ufw deny 23`
4.  **Test the rule**
    -   Try connecting to port 23 locally or remotely
5.  **Allow SSH (port 22) on Linux**
    -   `sudo ufw allow 22`
6.  **Remove test block rule**
    -   `sudo ufw delete deny 23`
7.  **Document commands/steps with screenshots**

## Summary

Firewalls filter traffic by applying rules that allow or block specific
connections.\
They are essential for protecting systems against unauthorized access.\
In this task, blocking Telnet (port 23) while allowing SSH (port 22)
demonstrated basic firewall management.
