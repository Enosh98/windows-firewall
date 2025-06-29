# windows-firewall
TASK 4
Task 4: Firewall Rule Configuration
🔒 Objective:
Use firewall settings to block and allow specific ports, test their effect, and understand traffic filtering.

🪟 Platform Used:
Windows 10
Firewall Tool: Windows Defender Firewall with Advanced Security
Additional Tool: Telnet (installed manually)

🔧 Steps Followed:
1. Opened the Firewall Configuration Tool
Searched for "Windows Defender Firewall with Advanced Security" from Start Menu.
2. Listed Current Rules
Explored Inbound and Outbound rules.
3. Blocked Port 23 (Telnet)
Created a new inbound rule:
Port: TCP, Port number: 23
Action: Block the connection
Applied to: Domain, Private, Public
Name: Block Telnet Port 23
4. Tested Block Rule
Enabled Telnet using:
dism /online /Enable-Feature /FeatureName: TelnetClient
Ran:
telnet localhost 23
Allowed Port 22 (SSH) Created another inbound rule:
Port: TCP 22

Action: Allow the connection

Name: Allow SSH Port 22 6. Removed Block Rule Located Block Telnet Port 23 in Inbound Rules.

Right-clicked → Deleted to restore original state. 📄 Commands Used: dism /online /Enable-Feature /FeatureName: TelnetClient telnet localhost 23

<img width="602" alt="460076002-b8194431-8169-4645-ae35-0e3cc8038753" src="https://github.com/user-attachments/assets/59dd7126-4b51-476c-9192-48af6c790b40" />
