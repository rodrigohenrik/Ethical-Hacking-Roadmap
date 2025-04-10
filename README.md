<p align="center">
    <a href="https://github.com/rodrigohenrik/Ethical-Hacking-Roadmap/"<img src="https://i.imgur.com/1PmMhIr.png" alt="Ethical Hacking Roadmap" /></a><br>
</p>

# ✅ Ethical Hacking Roadmap

This repository is a comprehensive guide for anyone looking to learn **penetration testing** and **ethical hacking** — from beginner to advanced. You'll find a structured learning path, essential tools, curated resources, and references to practice hacking legally and responsibly.

Most of the tools included are **UNIX-compatible**, **free**, and **open source**.

## 📌 What’s inside:
- Step-by-step learning roadmap (theory + hands-on practice)  
- Essential tools for each stage of penetration testing  
- Links to labs, books, CTFs, and cheatsheets  
- Content tailored for both beginners and those looking to go deeper

> ⚠️ **This project is intended for educational and ethical purposes only.** Use responsibly.

## Status

**This project is constantly being updated**. Some content may be out of date. **(Last revision:** April 9, 2025)

----

## Before you start

- If you're new to information security, forget everything you know about hacking.
- Don't start using tools without reading about pen testing and how it works *(see [Additional resources](#additional-resources) section)*.
- Don't download or use tools without auditing their code.
- Don't use these tools to do stupid things like investigating/hacking without consent on your friends, or worse, your recruiter.
- Read books, manuals, and articles, be curious, and do not just be a [script kiddie](https://www.wikihow.com/Avoid-Becoming-a-Script-Kiddie).
- I wish you wouldn't use these tools for illegal purposes, but if you do, I sure hope you know what you're doing.
- Practice using [challenges](#challenges), not real targets!

# 📄 Index / Table of Contents

- [Introduction](#introduction)
  - [What is penetration testing?](#what-is-penetration-testing)
  - [Want to become a penetration tester?](#want-to-become-a-penetration-tester)
- [Some Ethical Hacking Terms](#some-ethical-hacking-terms)
- [Difference Between Hacking and Ethical Hacking](#difference-between-hacking-and-ethical-hacking)
- [Languages](#languages)
- [Content Management Systems](#content-management-systems)
- [Basic Steps of Penetration Testing](#basic-steps-of-penetration-testing)
- [Tools by Category](#tools-by-category)
  - [:male_detective: Information Gathering](#male_detective-information-gathering)
  - [:lock: Password Attacks](#lock-password-attacks)
    - [:memo: Wordlists](#memo-wordlists)
  - [:globe_with_meridians: Wireless Testing](#globe_with_meridians-wireless-testing)
  - [:wrench: Exploitation Tools](#wrench-exploitation-tools)
  - [:busts_in_silhouette: Sniffing & Spoofing](#busts_in_silhouette-sniffing--spoofing)
  - [:rocket: Web Hacking](#rocket-web-hacking)
  - [:tada: Post Exploitation](#tada-post-exploitation)
  - [:package: Frameworks](#package-frameworks)
- [Additional Resources](#additional-resources)
  - [Education](#education)
  - [YouTube](#youtube)
  - [Books / Manuals](#books--manuals)
  - [Discussions](#discussions)
  - [News](#news)
  - [Blogs](#blogs)
  - [Security Advisories](#security-advisories)
  - [Challenges](#challenges)
- [License](#license)

*TOC made with: [nGitHubTOC](https://imthenachoman.github.io/nGitHubTOC/)*

# 💎 Introduction

## What is penetration testing?

Penetration testing is a type of security testing that is used to test the security of an application. It is conducted to find a security risk that might be present in a system.

If a system is not secure, then an attacker may be able to disrupt or take unauthorized control of that system. A security risk is normally an accidental error that occurs while developing and implementing software. For example, configuration errors, design errors, and software bugs etc. *[Learn more](https://www.tutorialspoint.com/penetration_testing/penetration_testing_quick_guide.htm)*

### Here's a quick breakdown:

- **Purpose**: To find security weaknesses before a real attacker does.
- **Method**: Ethical hackers (also called **white-hat hackers** or **pen testers**) mimic the tactics and techniques of malicious hackers.
- **Scope**: It can include testing web applications, internal/external networks, wireless networks, mobile apps, or physical security.

### Types of Penetration Testing:

1. **Black Box**: Tester has no prior knowledge of the system.
2. **White Box**: Tester has full knowledge, including source code and infrastructure.
3. **Gray Box**: Tester has partial knowledge (like a user with some access).

### Common Steps in a Pen Test:

1. **Reconnaissance** – Gather information about the target.
2. **Scanning** – Identify open ports, services, and vulnerabilities.
3. **Exploitation** – Try to break in using identified weaknesses.
4. **Post-exploitation** – Assess the impact (e.g., can data be stolen or systems controlled?).
5. **Reporting** – Document findings and provide remediation recommendations.

### Why It's Important:

- Prevents data breaches
- Helps meet compliance requirements (e.g., PCI-DSS, HIPAA)
- Builds trust with customers and stakeholders

## Want to become a penetration tester?

Knowing about risks on the internet and how they can be prevented is very useful, especially as a developer. Web hacking and penetration testing is the v2.0 of self-defense! But is knowing about tools and how to use them all you need to become a pen tester? Surely not. A real penetration tester must be able to proceed rigorously and detect the weaknesses of an application. They must be able to identify the technology behind and test every single door that might be open to hackers.

This repository aims first to establish a reflection method on penetration testing and explain how to proceed to secure an application. And secondly, to regroup all kinds of tools or resources that pen testers need. **Be sure to know the basics of programming languages and internet security before learning pen testing.**

Also, this is important to inform yourself about the law and what you are allowed to do or not. According to your country, the computer laws are not the same. First, check laws about privacy and surveillance: [Nine eyes countries](https://en.wikipedia.org/wiki/Five_Eyes#Other_international_cooperatives), [Five eyes](https://en.wikipedia.org/wiki/Five_Eyes), and [Fourteen Eyes](https://en.wikipedia.org/wiki/Five_Eyes#Fourteen_Eyes). Always check if what you're doing is legal. Even when it's not offensive, information gathering can also be illegal!

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 📌 Some Ethical Hacking Terms

- **Infosec**: Information security, which is the practice of preventing unauthorized access, use, disclosure, disruption, modification, inspection, recording, or destruction of information. The information or data may take any form, e.g., electronic or physical. Infosec can also be a person who practices ethical security. [Wikipedia](https://en.wikipedia.org/wiki/Information_security)

- **Opsec**: Operations security, which is a process that identifies critical information to determine if friendly actions can be observed by enemy intelligence, determines if information obtained by adversaries could be interpreted to be useful to them, and then executes selected measures that eliminate or reduce adversary exploitation of friendly critical information. [Wikipedia](https://en.wikipedia.org/wiki/Operations_security)

- **Black/grey/white hat hacker**: Someone who uses bugs or exploits to break into systems or applications. The goal and the method differ depending on whether they're a black, grey, or white hat hacker. A black hat is just someone malicious who does not wait  for permission to break into a system or application. A white hat is *usually* a security researcher who practices ethical hacking. A grey hat is just in the middle of these two kinds of hackers, they might want to be malicious if it can be beneficial (data breach, money, whistleblowing...).

- **Red team**: According to Wikipedia, a red team or the red team is an independent group that challenges an organization to improve its effectiveness by assuming an adversarial role or point of view. It is particularly effective in organizations with strong cultures and fixed ways of approaching problems. The United States intelligence community (military and civilian) has red teams that explore alternative futures and write articles as if they were foreign world leaders. Little formal doctrine or publications about Red Teaming in the military exist. In infosec exercises, Red teamers are playing the role of attackers. [Wikipedia](https://en.wikipedia.org/wiki/Red_team)

- **Blue team**: A blue team is a group of individuals who perform an analysis of information systems to ensure security, identify security flaws, verify the effectiveness of each security measure, and ensure certain all security measures will continue to be effective after implementation. As a result, blue teams were developed to design defensive measures against red team activities. In infosec exercises, Blue teamers are playing the role of defenders. [Wikipedia](https://en.wikipedia.org/wiki/Blue_team_(computer_security))

- **Penetration tester**: An ethical hacker who practices security, tests applications and systems to prevent intrusions or find vulnerabilities. [Wikipedia](https://en.wikipedia.org/wiki/Penetration_test)

- **Security researcher**: Someone who practices pen testing and browses the web to find phishing/fake websites, infected servers, bugs, or vulnerabilities. They can work for a company as a security consultant and are most likely a Blue teamer. [Wikipedia](https://en.wikipedia.org/wiki/Security_hacker)

- **Reverse engineering**: Reverse engineering, also called back engineering, is the process by which a man-made object is deconstructed to reveal its designs, architecture, or to extract knowledge from the object. Similar to scientific research, the only difference is that scientific research is about a natural phenomenon. [Wikipedia](https://en.wikipedia.org/wiki/Reverse_engineering)

- **Social engineering**: In the context of information security, it refers to psychological manipulation of people into performing actions or divulging confidential information. A type of confidence trick for information gathering, fraud, or system access, it differs from a traditional "con" in that it is often one of many steps in a more complex fraud scheme. The term "social engineering" as an act of psychological manipulation of a human is also associated with the social sciences, but its usage has caught on among computer and information security professionals. [Wikipedia](https://en.wikipedia.org/wiki/Social_engineering_(security))

- **Threat analyst**: A threat hunter, also called a cybersecurity threat analyst, is a security professional or managed service provider (MSP) that proactively uses manual or machine-assisted techniques to detect security incidents that may elude the grasp of automated systems. Threat hunters aim to uncover incidents that an enterprise would otherwise not find out about, providing chief information security officers (CISOs) and chief information officers (CIOs) with an additional line of defense against advanced persistent threats (APTs). [SearchCIO](https://searchcio.techtarget.com/definition/threat-hunter-cybersecurity-threat-analyst)

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 💻 Difference Between Hacking and Ethical Hacking

While both hackers and ethical hackers use similar techniques and skills, their intentions and goals are fundamentally different.

A black hat hacker engages in hacking for malicious purposes—stealing data, damaging systems, or gaining unauthorized access. In contrast, a white hat hacker, also known as an ethical hacker, uses the same knowledge to help organizations strengthen their security.

Ethical hacking involves identifying vulnerabilities in systems, networks, or applications and helping fix them before they can be exploited by attackers. It is a legal and authorized activity carried out with the goal of improving cybersecurity.

An ethical hacker is essentially a security expert who thinks like a hacker—but acts with permission and integrity. They simulate real-world attacks to test defenses and ensure that systems are as secure as possible.

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 🔠 Languages

Learning programming is one of the best ways to begin your journey into cybersecurity. Understanding how code works helps you spot vulnerabilities, write tools, and automate tasks.

Many beginners start with **Python**—it’s widely used, beginner-friendly, and powerful for scripting, automation, and building security tools. Other languages like **PHP** and **Go** are less commonly used in security, but they still have their place depending on the context and goals.

**Scripting languages** like **Bash** (for Linux) and **PowerShell** (for Windows) are essential for writing automation scripts and command-line utilities, especially in system administration and penetration testing tasks.

It’s also important to understand how different languages operate:

- **Compiled languages** (e.g., **C++**, **Java**) are converted into machine code before execution. They’re typically faster and used for performance-critical applications.
- **Interpreted languages** (e.g., **Python**, **PHP**) run line by line via an interpreter, which can make development and debugging faster and easier.

Each language also comes with its own design patterns and best practices. Choosing the right language depends on what you're trying to build or learn—whether it's automation scripts, exploits, web tools, or system-level programming.

### Scripting

- Bash
- Powershell

### Software & mobile apps

- Java
- Swift
- C / C++ / C#

### General purpose

- Python
- Ruby
- Perl
- PHP
- Go

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 📝 Content Management Systems

Content Management Systems (CMS) are platforms that allow users to create, manage, and modify digital content with ease — often without needing to code.

## Popular CMS Platforms:

- **WordPress** – The most widely used CMS in the world, known for its flexibility, ease of use, and a vast ecosystem of plugins and themes.
- **Joomla!** – A powerful CMS that offers more built-in features than WordPress, ideal for users with some technical experience.
- **Drupal** – A highly customizable and secure CMS preferred by developers and large-scale websites needing complex data structures.
- **SPIP** – A French-language-oriented CMS designed for collaborative publishing, often used by academic and cultural organizations.

These are the most used Content Management Systems (CMS). See a complete list [here](https://en.wikipedia.org/wiki/List_of_content_management_systems).

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 💡 Basic Steps of Penetration Testing

1. **Planning & Reconnaissance**
   - Define scope, goals, and rules of engagement
   - Gather information (open-source intelligence, DNS info, IPs, etc.)

2. **Scanning & Enumeration**
   - Identify live hosts, open ports, and services
   - Use tools like Nmap, Nessus, or Nikto to gather details about systems
   - Enumerate users, shares, and system banners

3. **Gaining Access**
   - Exploit vulnerabilities to gain initial access
   - Techniques: SQL injection, password cracking, buffer overflows, etc.
   - Tools: Metasploit, SQLmap, Hydra, etc.

4. **Maintaining Access**
   - Install backdoors or create persistent accounts
   - Simulate APT (Advanced Persistent Threat) behavior
   - Optional based on test type and agreement

5. **Privilege Escalation**
   - Elevate access from user-level to admin/root
   - Techniques: Exploiting weak configs, misconfigurations, or kernel vulnerabilities

6. **Post-Exploitation & Data Extraction**
   - Assess the value of the compromised system
   - Extract sensitive data, test lateral movement to other systems
   - Understand the potential impact of a real breach

7. **Covering Tracks (optional)**
   - Clear logs and remove artifacts (used to simulate real attackers)
   - Only done if explicitly permitted in the rules of engagement

8. **Reporting & Remediation**
   - Document findings, exploited vulnerabilities, and recommendations
   - Provide technical and non-technical reports for different stakeholders
   - May include proof of concept (PoC) and fix suggestions

## The Penetration Testing Steps

<p align="center">
    <img src="https://i.imgur.com/W9fI75p.png">
</p>

*Image source: [How to Perform Network Penetration Testing in 2025](https://www.stationx.net/how-to-perform-network-penetration-testing/)*.

➡️ [Read more about Penetration Testing here!](https://www.tutorialspoint.com/penetration_testing/index.htm)

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 🛠️ Tools by Category

A more complete list of tools can be found on the [Kali Linux official website](https://www.kali.org/tools/).

### :male_detective: Information Gathering

Information Gathering tools allow you to collect host metadata about services and users. Check informations about a domain, IP address, phone number or an email address.

| Tool        | Language           | Support  | Description    |
| ----------- |-------------------------|----------|----------------|
| [theHarvester](https://github.com/laramies/theHarvester)      | **Python** | `Linux/Windows/macOS` | E-mails, subdomains and names Harvester. |
| [CTFR](https://github.com/UnaPibaGeek/ctfr)      | **Python** | `Linux/Windows/macOS` | Abusing Certificate Transparency logs for getting HTTPS websites subdomains. |
| [Sn1per](https://github.com/1N3/Sn1per)      | **bash** | `Linux/macOS` | Automated Pentest Recon Scanner. |
| [RED Hawk](https://github.com/Tuhinshubhra/RED_HAWK)      | **PHP** | `Linux/Windows/macOS` | All in one tool for Information Gathering, Vulnerability Scanning and Crawling. A must-have tool for all penetration testers. |
| [Infoga](https://github.com/m4ll0k/Infoga)      | **Python** | `Linux/Windows/macOS` | Email Information Gathering. |
| [KnockMail](https://github.com/4w4k3/KnockMail)      | **Python** | `Linux/Windows/macOS` | Check if email address exists. |
| [a2sv](https://github.com/hahwul/a2sv)      | **Python** | `Linux/Windows/macOS` | Auto Scanning to SSL Vulnerability. |
| [Wfuzz](https://github.com/xmendez/wfuzz)      | **Python** | `Linux/Windows/macOS` | Web application fuzzer. |
| [Nmap](https://github.com/nmap/nmap)      | **C/C++** | `Linux/Windows/macOS` | A very common tool. Network host, vuln, and port detector. |
| [PhoneInfoga](https://github.com/sundowndev/PhoneInfoga)      | **Go** | `Linux/macOS` | An OSINT framework for phone numbers. |

### :lock: Password Attacks

Crack passwords and create wordlists.

| Tool        | Language           | Support  | Description    |
| ----------- |-------------------------|----------|----------------|
| [John the Ripper](https://github.com/magnumripper/JohnTheRipper)      | **C** | `Linux/Windows/macOS` | John the Ripper is a fast password cracker. |
| [hashcat](https://github.com/hashcat/hashcat)      | **C** | `Linux/Windows/macOS` | World's fastest and most advanced password recovery utility. |
| [Hydra](https://github.com/vanhauser-thc/thc-hydra)      | **C** | `Linux/Windows/macOS` | Parallelized login cracker which supports numerous protocols to attack. |
| [ophcrack](https://gitlab.com/objectifsecurite/ophcrack)      | **C++** | `Linux/Windows/macOS` | Windows password cracker based on rainbow tables. |
| [Ncrack](https://github.com/nmap/ncrack)      | **C** | `Linux/Windows/macOS` | High-speed network authentication cracking tool. |
| [WGen](https://github.com/agusmakmun/Python-Wordlist-Generator)      | **Python** | `Linux/Windows/macOS` | Create awesome wordlists with Python. |
| [SSH Auditor](https://github.com/ncsa/ssh-auditor)      | **Go** | `Linux/macOS` | The best way to scan for weak SSH passwords on your network. |

##### :memo: Wordlists

| Tool        | Description    |
| ----------- |----------------|
| [Probable Wordlist](https://github.com/berzerk0/Probable-Wordlists)      | Wordlists sorted by probability created for password generation and testing. |

### :globe_with_meridians: Wireless Testing

Used for intrusion detection and wifi attacks.

| Tool        | Language           | Support  | Description    |
| ----------- |-------------------------|----------|----------------|
| [Aircrack](https://github.com/aircrack-ng/aircrack-ng)      | **C** | `Linux/Windows/macOS` | WiFi security auditing tools suite. |
| [bettercap](https://github.com/bettercap/bettercap)      | **Go** | `Linux/Windows/macOS/Android` | bettercap is the Swiss army knife for network attacks and monitoring. |
| [WiFi Pumpkin](https://github.com/P0cL4bs/WiFi-Pumpkin)      | **Python** | `Linux/Windows/macOS/Android` | Framework for Rogue Wi-Fi Access Point Attack. |
| [Airgeddon](https://github.com/v1s1t0r1sh3r3/airgeddon)      | **Shell** | `Linux/Windows/macOS` | This is a multi-use bash script for Linux systems to audit wireless networks. |
| [Airbash](https://github.com/tehw0lf/airbash)      | **C** | `Linux/Windows/macOS` | A POSIX-compliant, fully automated WPA PSK handshake capture script aimed at penetration testing. |

### :wrench: Exploitation Tools

Access systems and data with service-oriented exploits.

| Tool                                                    | Language   | Support               | Description                                                  |
| ------------------------------------------------------- | ---------- | --------------------- | ------------------------------------------------------------ |
| [SQLmap](https://github.com/sqlmapproject/sqlmap)       | **Python** | `Linux/Windows/macOS` | Automatic SQL injection and database takeover tool.          |
| [XSStrike](https://github.com/UltimateHackers/XSStrike) | **Python** | `Linux/Windows/macOS` | Advanced XSS detection and exploitation suite.               |
| [Commix](https://github.com/commixproject/commix)       | **Python** | `Linux/Windows/macOS` | Automated All-in-One OS command injection and exploitation tool.￼ |
| [Nuclei](https://github.com/projectdiscovery/nuclei)    | **Go**     | `Linux/Windows/macOS` | Fast and customisable vulnerability scanner based on simple YAML-based DSL. |

### :busts_in_silhouette: Sniffing & Spoofing

Listen to network traffic or fake a network entity.

| Tool        | Language           | Support  | Description    |
| ----------- |-------------------------|----------|----------------|
| [Wireshark](https://www.wireshark.org)      | **C/C++** | `Linux/Windows/macOS` | Wireshark is a network protocol analyzer. |
| [WiFi Pumpkin](https://github.com/P0cL4bs/WiFi-Pumpkin)      | **Python** | `Linux/Windows/macOS/Android` | Framework for Rogue Wi-Fi Access Point Attack. |
| [Zarp](https://github.com/hatRiot/zarp)      | **Python** | `Linux/Windows/macOS` | A free network attack framework. |

### :rocket: Web Hacking

Exploit popular CMSs that are hosted online.

| Tool        | Language           | Support  | Description    |
| ----------- |-------------------------|----------|----------------|
| [WPScan](https://github.com/wpscanteam/wpscan)      | **Ruby** | `Linux/Windows/macOS` | WPScan is a black box WordPress vulnerability scanner. |
| [Droopescan](https://github.com/droope/droopescan)      | **Python** | `Linux/Windows/macOS` | A plugin-based scanner to identify issues with several CMSs, mainly Drupal & Silverstripe. |
| [Joomscan](https://github.com/rezasp/joomscan)      | **Perl** | `Linux/Windows/macOS` | Joomla Vulnerability Scanner. |
| [Drupwn](https://github.com/immunIT/drupwn)      | **Python** | `Linux/Windows/macOS` | Drupal Security Scanner to perform enumerations on Drupal-based web applications. |
| [CMSeek](https://github.com/Tuhinshubhra/CMSeek)      | **Python** | `Linux/Windows/macOS` | CMS Detection and Exploitation suite - Scan WordPress, Joomla, Drupal, and 130 other CMSs. |

### :tada: Post Exploitation

Exploits for after you have already gained access.

| Tool        | Language           | Support  | Description    |
| ----------- |-------------------------|----------|----------------|
| [TheFatRat](https://github.com/Screetsec/TheFatRat)      | **C** | `Linux/Windows/macOS` | Easy tool to generate backdoor and easy tool to post exploitation attack like browser attack, dll. |

### :package: Frameworks

Frameworks are packs of pen testing tools with custom shell navigation and documentation.

| Tool        | Language           | Support  | Description    |
| ----------- |-------------------------|----------|----------------|
| [Operative Framework](https://github.com/graniet/operative-framework)      | **Python** | `Linux/Windows/macOS` | Framework based on fingerprint action, this tool is used to get information on a website or an enterprise target with multiple modules. |
| [Metasploit](https://github.com/rapid7/metasploit-framework)      | **Ruby** | `Linux/Windows/macOS` | A penetration testing framework for ethical hackers. |
| [cSploit](https://github.com/cSploit/android)      | **Java** | `Android` | The most complete and advanced IT security professional toolkit on Android. |
| [radare2](https://github.com/radare/radare2)      | **C** | `Linux/Windows/macOS/Android` | Unix-like reverse engineering framework and commandline tools. |
| [Wifiphisher](https://github.com/wifiphisher/wifiphisher)      | **Python** | `Linux` | The Rogue Access Point Framework. |
| [Beef](https://github.com/beefproject/beef)      | **Javascript** | `Linux/Windows/macOS` | The Browser Exploitation Framework. It is a penetration testing tool that focuses on the web browser. |
| [Mobile Security Framework (MobSF)](https://github.com/MobSF/Mobile-Security-Framework-MobSF)      | **Python** | `Linux/Windows/macOS` | Mobile Security Framework (MobSF) is an automated, all-in-one mobile application (Android/iOS/Windows) pen-testing, malware analysis and security assessment framework capable of performing static and dynamic analysis. |
| [Burp Suite](https://portswigger.net/burp)      | **Java** | `Linux/Windows/macOS` | Burp Suite is a leading range of cybersecurity tools, brought to you by PortSwigger. **This tool is not free and open source** |

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 💼 Additional Resources

- [Awesome-Hacking Lists](https://github.com/Hack-with-Github/Awesome-Hacking)
- [The Life of a Security Researcher](https://www.alienvault.com/blogs/security-essentials/the-life-of-a-security-researcher)
- [Find awesome hacking spots in your country](https://github.com/diasdavid/awesome-hacking-spots)
- [Don't use VPN services](https://gist.github.com/joepie91/5a9909939e6ce7d09e29)
- [How to Avoid Becoming a Script Kiddie](https://www.wikihow.com/Avoid-Becoming-a-Script-Kiddie)
- [OWASP Top 10 Non-Human Identities Risks - 2025](https://owasp.org/www-project-non-human-identities-top-10/2025/top-10-2025/)
- [Starting in cybersecurity?](https://blog.0day.rocks/starting-in-cybersecurity-5b02d827fb54)
- [Crack Station](http://crackstation.net/)
- [Exploit Database](http://www.exploit-db.com/)
- [Hackavision](http://www.hackavision.com/)
- [Hackmethod](https://www.hackmethod.com/)
- [Smash the Stack](http://smashthestack.org/)
- [SecLists](http://seclists.org/)
- [SecTools](http://sectools.org/)

## Education

- [Cyber Security Expert](https://roadmap.sh/cyber-security) (Roadmap.sh)
- [Cyber Security Tutorial](https://www.tutorialspoint.com/cybersecurity/index.htm)
- [Ethical Hacking in 12 Hours - Full Course - Learn to Hack!](https://www.youtube.com/watch?v=fNzpcB7ODxQ) (The Cyber Mentor)
- [Full Ethical Hacking Course - Network Penetration Testing for Beginners (2019)](https://www.youtube.com/watch?v=3Kq1MIfTWCE&list=PLWKjhJtqVAbnklGh3FNRLECx_2D_vK3mu) (freeCodeCamp.org)
- [Developer Roadmaps](https://roadmap.sh/)

## YouTube

- [Ryan Montgomery](https://www.youtube.com/@0dayCTF)
- [The hacker’s roadmap (how to get started in IT in 2025)](https://www.youtube.com/watch?v=5xWnmUEi1Qw) (NetworkChuck)
- [2025 Ethical Hacker Roadmap with lots of free training (NOT Sponsored)](https://www.youtube.com/watch?v=OCjh8AULc8Y) (David Bombal)

## Books / Manuals

- [Kali Docs](https://www.kali.org/docs/)
- [Penetration Testing: A Hands-On Introduction to Hacking](https://www.amazon.com/Penetration-Testing-Hands-Introduction-Hacking/dp/1593275641) (2014)
- [Kali Linux Revealed](https://www.amazon.com/Kali-Linux-Revealed-Penetration-Distribution/dp/0997615605) (2017)
- [Blue Team Field Manual (BTFM)](https://www.amazon.com/Blue-Team-Field-Manual-BTFM/dp/154101636X) (2017)
- [Cybersecurity - Attack and Defense Strategies](https://www.amazon.com/Cybersecurity-Defense-Strategies-Infrastructure-security/dp/1788475291) (2018)
- [NMAP Network Scanning: Official Discovery](https://www.amazon.com/Nmap-Network-Scanning-Official-Discovery/dp/0979958717) (2009)
- [Social Engineering: The Art of Human Hacking](https://www.amazon.com/Social-Engineering-Art-Human-Hacking/dp/0470639539) (2010)
- [Incognito Toolkit: Tools, Apps, and Creative Methods for Remaining Anonymous](https://www.amazon.com/Incognito-Toolkit-Communicating-Publishing-Researching/dp/0985049146) (2013)

## Discussions

- [Reddit/HowToHack](https://www.reddit.com/r/HowToHack/) - Learn and ask about hacking, security, and pen testing.
- [Reddit/hacking](https://www.reddit.com/r/hacking) - Discuss about hacking and web security.
- [Reddit/AskNetsec](https://www.reddit.com/r/AskNetsec/) - Discuss network security, ask professionals for advice about jobs and stuff.
- [Reddit/cybersecurity](https://www.reddit.com/r/cybersecurity/) - Discuss cybersecurity news, research, threats, etc.

## News

- [The Hacker News](https://thehackernews.com/)
- [WeLiveSecurity](https://www.welivesecurity.com/en/)
- [Hacker News](https://news.ycombinator.com/)
- [Hackerday](https://hackaday.com/blog/)
- [HackerOne](https://www.hackerone.com/blog)
- [Latest Hacking News](https://latesthackingnews.com/)
- [Hackread](https://hackread.com/)

## Blogs

- [70 Best Hacker Blogs and Websites in 2025](https://bloggers.feedspot.com/hacker_blogs/) (FeedSpot)

## Security Advisories

- [CVE](http://cve.mitre.org/) - Official portal of the CVE program, which catalogs publicly known cybersecurity vulnerabilities by assigning unique identifiers (CVE IDs) to facilitate management and communication among security organizations.
- [CWE](http://cwe.mitre.org/) - Official portal of the CWE program, which categorizes common software and hardware weaknesses to help organizations identify, understand, and mitigate security flaws using a standardized framework.
- [NVD](http://web.nvd.nist.gov/) - Official portal of the National Vulnerability Database (NVD), a U.S. government repository managed by NIST that catalogs publicly known cybersecurity vulnerabilities, providing standardized data to support automated vulnerability management, security measurement, and compliance.

## Challenges

- [Vulnhub](https://www.vulnhub.com/) - Has a lot of VMs to play with. Some are beginner-friendly, some aren't.
- [Itsecgames](http://www.itsecgames.com/) - bWAPP or buggy web app is a deliberately insecure web application.
- [Hackthissite](https://www.hackthissite.org/) - A site which provides challenges, CTFs, and more to improve your hacking skills.
- [Defend the Web](https://defendtheweb.net/) - Defend the Web is an interactive security platform where you can learn and challenge your skills.
- [Root-me](https://www.root-me.org/) - Another website that hosts challenges to test your hacking skills.
- [HackTheBox](https://www.hackthebox.eu/) - An online platform to test and advance your skills in penetration testing and cybersecurity.
- [Overthewire](http://overthewire.org/wargames/) - Learn and practice security concepts in the form of fun-filled games.
- [Ctftime](https://ctftime.org/) - The de facto website for everything CTF related. 
- [TryHackMe](https://tryhackme.com/) - TryHackMe is a free online platform for learning cybersecurity, using hands-on exercises and labs.
- [PicoCTF](https://picoctf.org/) - Provides you with fun CTF challenges of varying levels of difficulty to practice on.

[*Go to the index*](#-index--table-of-contents) 👆🏻

# 💎 License

This repository is under the [MIT license](https://github.com/rodrigohenrik/Ethical-Hacking-Roadmap/blob/master/LICENSE).

[*Go to the index*](#-index--table-of-contents) 👆🏻
