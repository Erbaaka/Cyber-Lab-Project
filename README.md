# Cybersecurity Lab Project #1 - Attack Simulation & Monitoring

## Project Overview
Simulated cyber attack using **Kali Linux** against **Ubuntu**, with monitoring using **Wazuh SIEM**. The goal of this project is to understand the end-to-end process of cyber attack detection and analysis, from exploitation to logging and monitoring.

## Tools and Technology
- Kali Linux = OS for ethical hacking, penetration testing, and attack simulation.
- Ubuntu = Target OS
- Wazuh OVA = Monitoring system and SIEM
- Virtualbox = Local network attack (virtualization)

## Project Setup
1. Setup 3 virtual machine (Kali Linux, Wazuh, Ubuntu) to the same network. Wazuh & Ubuntu will be set up using Bridged Adapter and Kali Linux will be set up using NAT network.
2. Install Wazuh Agent in Ubuntu then connect it to Wazuh manager.
3. Login as an admin to Wazuh dashboard in Ubuntu.
4. Open terminal and use Hydra with 'rockyou.txt' wordlists to attack Ubuntu.
5. Look up and refresh Wazuh dashboard page.
6. Check on 'Last 24 hours alerts' section.
7. If the number are changed, the attack was successfully monitored by Wazuh.

## Result and Observation
Attack name | Status | Severity | Respond
- Credential brute force | Detected | Low and Medium Severity | Alert sent

## Lesson Learned
- Wazuh is effective in detecting common attacks such as brute force.
- The 'rockyou.txt' wordlist file have around 10000 wordlist.
- Duration of attack may vary.

## Documentation
Google Drive link : https://drive.google.com/file/d/1EtE4Q9lWCHPrE0um15hDXVsn0doLYSK_/view?usp=sharing

## References
- Wazuh Documentation (https://documentation.wazuh.com/)
- Hydra (https://www.kali.org/tools/hydra/)
- Wordlist (https://www.kali.org/tools/wordlists/)
