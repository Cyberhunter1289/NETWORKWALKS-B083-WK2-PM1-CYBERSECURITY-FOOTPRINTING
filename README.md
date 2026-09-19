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

TASK 1 - To Find the Public Domain Registration record of Networkwalks.com with the (whois tool) on Kali to get information like, Who owns the Domain, When it was Registered, and its Name Servers.

I have used the (whois tool) to reveal the registrar, registration and expiry dates, registrant details, and name servers of Networkwalks.com
  
![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20142413.png?raw=true?)

TASK 2 - To Fingerprint the Technologies running on the Networkwalks.com website e.g. Web Server, CMS, Plugins, Frameworks and IP Address

Using the (whatweb tool) to expose the web server, frameworks and IP address of Networkwalks.com

![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20144321.png?raw=true)

TASK 3 - To Resolve the domain name to its IP address using DNS.

nslookup allows me to turn Networkwalks.com domain name into its real IP address.

Knowing the target IP address let an attacker scan the server directly and map the target's infrastructure.

![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20144902.png?raw=true)

TASK 4 - To Read the HTTP Response Headers to see the Server Banner, Status, Cookies and Redirects.

I ran the curl -I tool to access the HTTP headers of Networkwalks.com which leak their web server, caching stack, and their hidden endpoints.

Attackers can read headers to fingerprint the stack and find entry points without even loading the full page.

![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20144932.png?raw=true)

TASK 5 - To Detect whether Networkwalks.com Web Application Firewall (WAF) is protecting their website.

I checked Networkwalks.com Web Application Firewall strength using the (wafw00f tool) which let me know that ModSecurity (SpiderLabs) is the kind of firewall protection used for their (WAF).

wafw00f let an attacker know if a firewall is watching, so that the attacker can be ready to bypass it.

![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20145011.png?raw=true)

TASK 6 - To Enumerate all DNS records: Name Servers, Mail Servers, SPF, TXT and Service (SRV) Records.

After gathering all the necessary information about Networkwalks.com through the Reconnaissance tools, we need to use (dnsrecon -d) to Enumerate all DNS records e.g. name server, SPF and service (SRV) records.

dnsrecon -d let attackers maps the target's entire DNS footprint which makes each record a potential foothold and helps an attacker understand the email and hosting setup.

![Image Alt](https://github.com/Cyberhunter1289/NETWORKWALKS-B083-WK2-PM1-CYBERSECURITY-FOOTPRINTING/blob/main/Screenshot%202026-09-18%20145822.png?raw=true)

NETWORKWALKS WEEK 2 PROJECT MODULE 1 (FOOOTPRINTING ON NETWORLWALKS.COM) DONE AND DUSTED.
