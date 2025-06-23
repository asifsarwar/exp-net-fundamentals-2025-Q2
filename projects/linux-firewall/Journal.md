## Linux FIrewall Rules

### Goal
I want to see how easy or difficult it is to manage GCP firewall rules and linux firewall rules.

### Considerations

I am launching Debian latest version of GCP,
I am not sure what is intalled by default.

## Investigation

- IPTables was already installed
- Python3 was already installed

I was able to edit the iptables through commands, direct editing iptables files wasn't possible and even if I could it's not recommended.

I could have used ufw but I wanted to get experience with iptables since on some machines I might not be allowed to install ufw packages.

## Outcomes

I was able to open port 7000, 8000 in GCP firewall rules.

I was able to use curl with a 2 second timeout and reach the website with port 8000

I was able to block port 8000 on iptables.

I was able to redirect form 7000 externally to 8000 using iptables.

I could not combine blocking port 8000 and redirecting port 7000 to port 8000 but I suspect its possible.

It seems that iptables is easy when utilizing an AI coding Assistant eg. ChatGPT so there is no need for ufw unless we didn't have access to an LLM and we wanted to simply use man to qucikly learn how to change rules or have an easy way to remember how to change rules.

![](/projects/linux-firewall/assets/block_port_8000_redirect_7000_to_8000.PNG)