# NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING (RECONNAISSANCE)
This is my Week 2 Networkwalks Project Module 1 - Footprinting (Reconnaissance) with Multiple Kali Tools e.g. Whois, Whatweb, Nslookup, Curl -I, Wafw00f and Dnsrecon -d for the Reconnaissance Attacks on Networkwalks.com

Reconnaissance (also known as footprinting) is the first step in any real attack or security test. Before touching a target, an attacker quietly collects as much public information about the target as possible. This includes who owns the domain, its real IP address, the hosting provider, the web technologies it runs, its DNS and mail records, and whether a firewall is protecting it. All of this OSINT comes from information the target has already made public, so the target never even knows it is being studied.

TASKS TO COMPLETE (ON NETWORKWALKS.COM)

Task 1. Run whois to find the domain registration details.

Task 2. Run whatweb to fingerprint the web technologies.

Task 3. Run nslookup to resolve the domain to its IP address.

Task 4. Run curl -I to read the HTTP response headers.

Task 5. Run wafw00f to detect a Web Application Firewall.

Task 6. Run dnsrecon to enumerate all DNS records.

  TASK 1 - Finding the Public Domain Registration record of Networkwalks.com with the (whois tool) on Kali to get information like, Who owns the Domain, When it was Registered, and its Name Servers.

  I have used the (whois tool) to reveal the registrar, registration and expiry dates, registrant details, and name servers of Networkwalks.com
  
![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20142413.png?raw=true?)

TASK 2 - Fingerprinting the Technologies running on the Networkwalks.com website e.g. Web Server, CMS, Plugins, Frameworks and IP Address

Using the (whatweb tool) to expose the web server, frameworks and IP address of Networkwalks.com

![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20144321.png?raw=true)

TASK 3 - Resolving the domain name to its IP address using DNS.

nslookup allows me to turn Networkwalks.com domain name into its real IP address.

Knowing the target IP address let an attacker scan the server directly and map the target's infrastructure.

![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20144902.png?raw=true)



