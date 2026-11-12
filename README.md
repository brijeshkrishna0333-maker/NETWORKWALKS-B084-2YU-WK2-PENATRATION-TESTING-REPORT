# NETWORKWALKS-B084-2YU-WK2-PENATRATION-TESTING-REPORT
Week 2 lab report from my cybersecurity internship at Networkwalks. Covers footprinting a website and scanning my own network with Kali Linux tools and Zenmap
Lab Report: What a Website and a Network Reveal About Themselves

Name:Brijesh Yellapu
Internship: Cybersecurity, Networkwalks IT Solutions & Training
Batch: B084
Date: 12/11/2026
Modules: Penatration Testing

1. Permission

I only tested systems I had permission to test. The website I looked at was , and I had approval to do this. The network I scanned was my own. I did not scan any device that belongs to someone else. This report is for learning only.

2. Overview

This lab had two tasks. First, I tried to learn as much as I could about a website using only public information. Second, I scanned my own network to see which devices were on it.

Attackers often begin this way: they look around first, then check what is connected. I only observed things this week. I did not try to get into anything.

3. Tools
Tool	Why I used it
WHOIS	To see who registered the domain
WhatWeb	To find out what technology the site uses
Nslookup	To get the site’s IP address
Curl -I	To read the information the server sends back
Wafw00f	To check for a web firewall
DNSRecon	To list the domain’s DNS records
ipconfig	To find my own IP address and subnet
Zenmap	To discover devices on my network
4. Steps and results
Task 1: The website
WHOIS: I looked up . It showed [registrar, dates, name servers].
WhatWeb: It reported [CMS, version, plugins, server]. 
Nslookup: The domain pointed to [IP address].
Curl -I: The headers showed [server details, extra info, any visible paths]. 
Wafw00f: The result was [firewall name or “none found”]. 
DNSRecon: It listed [name servers, mail servers, TXT/SPF records].
Task 2: My network

I ran ipconfig and found my IP  and my subnet . I entered the subnet in Zenmap and ran a Ping Scan, which found 3 devices.

I then opened the Topology tab, switched on the legend and saved the diagram as a PDF and i will be attaching it.

5. What the results might mean

These are observations, not proven weaknesses. I only collected information and did not test for vulnerabilities.

Observation	Why it could matter	Risk
Software and version visible	Someone could check it for known issues	[Low/Medium]
IP address easy to find	Shows where the site is hosted	[Low]
Technical details in headers	Small clues about the setup	[Low]
Firewall can be identified	Shows what protection exists	[Low]
DNS records are public	Reveals mail and other services	[Low/Medium]
Devices visible on the network	An unknown device could go unnoticed	[Low/Medium]


6. Recommendations
Remove technical details the website doesn’t need to show.
Keep the CMS, plugins and server software updated.
Review DNS records from time to time.
Keep the firewall switched on and properly set up.
Scan your own network now and then to spot unknown devices.
Keep an up-to-date list of your devices.
Get permission before testing anything.

7.What I learned

Before this week, I didn’t realise how much anyone can find out about a website without logging in or breaking anything. A few simple tools gave me the website’s software, its IP, its DNS records and whether it has a firewall.

The scan also showed me how quickly a network can be mapped. I’d never really thought about how many devices were on mine until I saw them in a list.

The other thing I learned is how to write things up. A good report says what I did, what I saw, why it matters and what to do about it. And none of this should ever be done without permission.

8. Conclusion
I was surprised by how much a few simple tools can show without logging in or breaking anything. The scan also showed me how quickly a network can be mapped.

I also learned that a good report explains what was done, what was seen, why it matters and what to do next. Most importantly, this kind of testing should only ever be done with permission.

8. Evidence

Screenshots: WHOIS, WhatWeb, Nslookup, Curl -I, Wafw00f, DNSRecon, ipconfig, Zenmap ping scan, plus the topology PDF.
