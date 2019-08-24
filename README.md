# Google Summer of Code 2019 - OWASP (Final Submission)

## Table of Contents

- [Overview](#overview)
    - [About me](#about-me)
    - [Project details](#project-details)
    - [Proposed summary](#proposed-summary)
    - [Work done](#work-done)

- [Contributions](#contributions)
    - [Pull requests and issues](#pull-requests-and-issues)
        - [Detailed view in Google docs (with links to the PR)](https://docs.google.com/document/d/1lUO-T9zKRGRVDdsmppv_8HJkTVPsfPT6wpmE1cKCLo8/edit?usp=sharing)
        - [Minimal view in Google spreadsheet (with links to the PR)](https://docs.google.com/spreadsheets/d/1nxuYSdYKabez0-pdhyYFtrExwJtUiiV2UoeCJGnf82o/edit?usp=sharing)
        - [View here](#view-here)
    - [Commits](#commits)
    - [Contribution graph and status](#contribution-graph-and-status)

- [Blog posts made](#blog-posts-made)

- [Screenshots screenscasts and tutorial videos](#screenshots-screenscasts-and-tutorial-videos)

- [Future work](#future-work)

- [Personal experience and journey](#personal-experience-and-journey)

- [Conclusion](#conclusion)

## Overview

### About Me

- **Name:** Abhishek Sharma
- **Major:** Computer Science & Engineering
- **University:** Chandigarh University
- **GitHub:** [@abhisharma404](https://github.com/abhisharma404)
- **E-mail:** abhishekchem98@gmail.com, abhishek_official@hotmail.com
- **Telegram ID:** abhisharma404
- **Personal website / blog:** https://abhisharma404.blogspot.com/
- **Project URL:** https://www.github.com/OWASP/SecureTea-Project<br>

### Project details

The OWASP SecureTea Project focuses on providing a one-stop security solution for various devices (personal computers / servers / IoT devices).

Currently the following features are supported:

- [x] Intrusion Detection System
- [x] Firewall
- [x] AntiVirus
- [x] Server Log Monitor
- [x] System Log Monitor
- [x] Local Web Deface Detection & Prevention System
- [x] Auto Web Server Patcher
- [x] IoT Anonymity checker
- [x] Auto report generation using OSINT
- [x] Notifying suspicious activities using various mediums (Twitter, Telegram, Slack, Gmail, SMS, AWS & more)
- [x] Interactive GUI for ease of setting up

**Organisation:** OWASP Foundation<br>
**Project URL:** https://www.github.com/OWASP/SecureTea-Project<br>
**IRC channel:** https://t.me/joinchat/Az5yZxQg7Djs-UZWKKCRVQ<br>
**Mentor:** Rejah Rehim [(@rejahrehim)](https://github.com/rejahrehim)<br>
**Proposal Title:** Laying down base architecture<br>
**Tag:** securetea tools<br>

### Proposed summary

**Proposed summary as per proposal**:

Laying down a strong foundation & base architecture for Intrusion detection & prevention system (IDS/IPS), intelligent log monitoring, antivirus that can be scaled in future and also can be further expanded easily by applying machine learning. Enhance the current firewall by bringing in some advanced rules to detect malformed & suspicious packets & dump them into a PCAP file for future forensic analysis. Implement OSINT tools to collect information about attackers and generate a CSV report. Introduce Auto Server patcher to patch server configuration for maximum security features and implement a server side web deface detection. Also, protect IoT devices by checking if they are under the Shodan radar. Perform all the elemental connections & introduce different modes for the user. Improve the GUI by adding all the configurations options and critical data such as last login to it. Perform bug fixes and improve the dashboard. Write a detailed documentation and readme, and finally package and ship SecureTea version 1.1 on PyPi.

### Work done

**Summary of the work done during the GSoC Phase (I - III):**

- Implemented Intrusion Detection System capable of detecting:
    - [DoS and R2L attacks](https://github.com/OWASP/SecureTea-Project/pull/102)
    - [Reconnaissance attacks](https://github.com/OWASP/SecureTea-Project/pull/101)
           
- Introduced advanced packet filter rules & PCAP dumping for Firewall:

    - [Improved the overall functionalities of the current firewall by adding new packet rules at
      IP, TCP & ICMP level to detect attacks like fragmentation, malicious and malformed
      packets, enable PCAP dumping of rejected packets](https://github.com/OWASP/SecureTea-Project/pull/104)
      
- [Implemented System Log Monitor capable of detecting un-authorized system manipulation and attacks](https://github.com/OWASP/SecureTea-Project/pull/126)

- [Implemented Server Log Monitor capable of processing Apache & Nginx log files to detect web attacks](https://github.com/OWASP/SecureTea-Project/pull/138)

- [Implemented AntiVirus by using signature scanning and incorporating other open source antivirus for heruistic scanning](https://github.com/OWASP/SecureTea-Project/pull/151)

- [Introduced SecureTea Auto Server Patcher to patch system and server configurations for maximum security features & overcome common deployment mistakes](https://github.com/OWASP/SecureTea-Project/pull/142)

- [Implemented Local web deface detection & prevention mechanism](https://github.com/OWASP/SecureTea-Project/pull/146)

- Brought intelligence to Firewall by making it learn bad IPs from:
    - [Intrusion Detection System](https://github.com/OWASP/SecureTea-Project/pull/183)
    - [System Log Monitor](https://github.com/OWASP/SecureTea-Project/pull/185)
    - [Server Log Monitor](https://github.com/OWASP/SecureTea-Project/pull/184)

- [Introduced Open Source Intelligence Tools (OSINT) tool](https://github.com/OWASP/SecureTea-Project/pull/152)

- Introduced auto detail collection of hackers using the bad IPs and OSINT tools as collected by:
    - [Intrusion Detection System](https://github.com/OWASP/SecureTea-Project/pull/181)
    - [Firewall](https://github.com/OWASP/SecureTea-Project/pull/179)
    - [System log Monitor](https://github.com/OWASP/SecureTea-Project/pull/182)
    - [Server Log Monitor](https://github.com/OWASP/SecureTea-Project/pull/180)

- [Introduced IoT Anonymity checker to protect IoT devices and check their visibility under the Shodan radar](https://github.com/OWASP/SecureTea-Project/pull/153)

- Performed elemental connections of elements & introduced 3 modes:
    - [Server mode](https://github.com/OWASP/SecureTea-Project/pull/187)
    - [System mode](https://github.com/OWASP/SecureTea-Project/pull/188)
    - [IoT mode](https://github.com/OWASP/SecureTea-Project/pull/190)

- Performed front-end Angular JS touch-ups
    - [View list of PRs](https://github.com/OWASP/SecureTea-Project/pulls?utf8=%E2%9C%93&q=GUI)

- [Added last logins to the GUI dashboard](https://github.com/OWASP/SecureTea-Project/pull/205)

- [Deployed GUI preview on Heroku](https://github.com/OWASP/SecureTea-Project/pull/236)

- [Guide to enable local web serving over HTTPS](https://github.com/OWASP/SecureTea-Project/pull/233)

- [Final packaging](https://github.com/OWASP/SecureTea-Project/pull/237)

- Performed bug fixes

- [Documentation - User guide & developer guide](https://github.com/OWASP/SecureTea-Project/issues?utf8=%E2%9C%93&q=docs+author%3Aabhisharma404)

- [Raised relevant issues](https://github.com/OWASP/SecureTea-Project/issues?q=is%3Aissue+author%3Aabhisharma404+is%3Aclosed)

## Contributions
### Pull requests and issues

- [Detailed view in Google docs (with links to the PR)](https://docs.google.com/document/d/1lUO-T9zKRGRVDdsmppv_8HJkTVPsfPT6wpmE1cKCLo8/edit?usp=sharing)

- [Minimal view in Google spreadsheet (with links to the PR)](https://docs.google.com/spreadsheets/d/1nxuYSdYKabez0-pdhyYFtrExwJtUiiV2UoeCJGnf82o/edit?usp=sharing)

- [View here](#view-here)

- [Commits](#commits)
    
#### View here
|Date            |Type        |Status|ID  |Name                                                                                                   |
|----------------|------------|------|----|-------------------------------------------------------------------------------------------------------|
|**Pre-GSoC**        |            |      |    |                                                                                                       |
|13.01.2019      |Issue       |Closed|#9  |Error while installing                                                                                 |
|13.01.2019      |Pull Request|Merged|#10 |Fix #9 setup error                                                                                     |
|13.01.2019      |Pull Request|Merged|#11 |Add badges, fixed typos & others                                                                       |
|14.01.2019      |Issue       |Closed|#12 |Bug : sudo pm-suspend does not work on Ubuntu 18.04                                                    |
|14.01.2019      |Pull Request|Merged|#13 |Fix pm-suspend in new releases of Ubuntu                                                               |
|26.01.2019      |Pull Request|Merged|#18 |Feature: SMS notification using Twilio API                                                             |
|28.01.2019      |Issue       |Closed|#21 |Bug: Python 3 not supported                                                                            |
|01.02.2019      |Pull Request|Merged|#23 |Reduce code crowding in core.py & introduce interactive setup                                          |
|01.02.2019      |Pull Request|Merged|#31 |Minor touchups                                                                                         |
|01.02.2019      |Issue       |Closed|#32 |Restructuring the current project architecture                                                         |
|04.02.2019      |Pull Request|Merged|#33 |Close #32 : Re-structured to group the common behavioral files                                         |
|18.02.2019      |Pull Request|Merged|#35 |Add SecureTea-Firewall                                                                                 |
|02.03.2019      |Pull Request|Merged|#39 |CLI configuration & interactive setup for Firewall                                                     |
|08.03.2019      |Pull Request|Merged|#41 |Add unit-tests                                                                                         |
|17.03.2019      |Pull Request|Merged|#45 |Improve Firewall: log xnor decorator error, check root state                                           |
|17.03.2019      |Pull Request|Merged|#46 |Improve unittest: Add support for mock-patch in Python 2                                               |
|17.03.2019      |Pull Request|Merged|#47 |Bringing continuous integration service to SecureTea                                                   |
|17.03.2019      |Pull Request|Merged|#48 |Close #43 - Add documentation                                                                          |
|17.03.2019      |Pull Request|Merged|#49 |Separate developer & user guide                                                                        |
|24.03.2019      |Pull Request|Merged|#60 |Add geo-location function                                                                              |
|26.03.2019      |Pull Request|Merged|#63 |Add insecure-headers feature                                                                           |
|26.03.2019      |Issue       |Closed|#65 |Bug: Lost support for Python 3 & failing test cases                                                    |
|26.03.2019      |Pull Request|Closed|#68 |Fix #65 : Restore Python 3 support & pass test cases                                                   |
|13.04.2019      |Pull Request|Closed|#84 |Add Gmail notification feature                                                                         |
|15.04.2019      |Pull Request|Closed|#85 |PEP-8 & other minor fixes                                                                              |
|20.04.2019      |Pull Request|Closed|#88 |Fix #52 - sqlite3 operational error                                                                    |
|20.04.2019      |Pull Request|Closed|#89 |Add libnetfilterqueue to pre-requisites                                                                |
|                |            |      |    |                                                                                                       |
|**GSoC Phase - I**  |            |      |    |                                                                                                       |
|12.05.2019      |Pull Request|Merged|#99 |Add unittest for AWS                                                                                   |
|15.05.2019      |Pull Request|Merged|#100|Add docstrings to un-documented functions/methods                                                      |
|18.05.2019      |Pull Request|Merged|#101|Add SecureTea IDS (recon)                                                                              |
|27.05.2019      |Pull Request|Merged|#102|Add R2L attack vectors to IDS                                                                          |
|27.05.2019      |Pull Request|Merged|#103|Update docs (user & dev guide)                                                                         |
|29.05.2019      |Pull Request|Merged|#104|Add advanced Firewall rules & enable PCAP dumping of rejected packets                                  |
|29.05.2019      |Pull Request|Merged|#105|Mock get_current_location API call                                                                     |
|30.05.2019      |Pull Request|Merged|#106|Minor fix                                                                                              |
|30.05.2019      |Pull Request|Merged|#107|Update user & developer guide                                                                          |
|31.05.2019      |Pull Request|Merged|#108|Update setup.py to latest                                                                              |
|31.05.2019      |Pull Request|Merged|#111|Update to setup.py to check for dependency                                                             |
|31.05.2019      |Pull Request|Merged|#113|Enable OS specific dependency installation                                                             |
|04.06.2019      |Pull Request|Merged|#123|Fix pytest travis error                                                                                |
|13.06.2019      |Pull Request|Merged|#126|Add system log monitor                                                                                 |
|11.06.2019      |Pull Request|Merged|#127|Update user docs to add system log monitor                                                             |
|06.06.2019      |Pull Request|Merged|#128|Create user guide for PyPi                                                                             |
|06.06.2019      |Issue       |Closed|#129|Bug: KeyError in AWS SES                                                                               |
|06.06.2019      |Pull Request|Merged|#130|Fix #129 AWS SES KeyError                                                                              |
|06.06.2019      |Issue       |Closed|#131|Bug: Gmail class destructor called before                                                              |
|06.06.2019      |Pull Request|Merged|#132|Fix #131 - Initialize before destruct                                                                  |
|06.06.2019      |Pull Request|Merged|#133|Fix Codacy warning - Handle exception                                                                  |
|06.06.2019      |Pull Request|Merged|#134|Add system log developer guide                                                                         |
|20.07.2019      |Pull Request|Merged|#172|PyPi docs: Add IoT checker docs                                                                        |
|20.07.2019      |Pull Request|Merged|#173|Update setup.py                                                                                        |
|20.07.2019      |Pull Request|Merged|#174|Dev docs: Update roadmap                                                                               |
|21.07.2019      |Pull Request|Merged|#175|Update developer docs                                                                                  |
|21.07.2019      |Pull Request|Merged|#176|Update setup.py for 1.5.1 release                                                                      |
|21.07.2019      |Pull Request|Merged|#177|User docs: Add OSINT feature details                                                                   |
|21.07.2019      |Pull Request|Merged|#178|PyPi: Add OSINT details                                                                                |
|                |            |      |    |                                                                                                       |
|**GSoC Phase - II** |            |      |    |                                                                                                       |
|18.06.2019      |Pull Request|Merged|#138|Feature: Add Server log monitor                                                                        |
|18.06.2019      |Pull Request|Merged|#139|Add server log documentation (user)                                                                    |
|18.06.2019      |Pull Request|Merged|#140|Add server log docs (PyPi)                                                                             |
|18.06.2019      |Pull Request|Merged|#141|Update setup.py for v1.4 release                                                                       |
|24.06.2019      |Pull Request|Merged|#142|Feature: Add Auto Server Patcher                                                                       |
|25.06.2019      |Pull Request|Merged|#143|Classify arguments for easier understanding                                                            |
|25.06.2019      |Pull Request|Merged|#144|Display list of interfaces                                                                             |
|30.06.2019      |Pull Request|Merged|#146|Feature: Add web deface detection (server side)                                                        |
|01.07.2019      |Pull Request|Merged|#147|Update user docs for auto-server-patcher                                                               |
|01.07.2019      |Pull Request|Merged|#148|Update PyPi user guide for auto-server-patcher & tabular view of arguments                             |
|01.07.2019      |Pull Request|Merged|#149|Update .gitignore to ignore temp PCAP files                                                            |
|15.07.2019      |Pull Request|Merged|#151|Add SecureTea Anti-Virus                                                                               |
|16.07.2019      |Pull Request|Merged|#152|Feature: OSINT analysis about the IP address                                                           |
|18.07.2019      |Pull Request|Merged|#153|Featrue: Check IoT device Security / Anonymity                                                         |
|18.07.2019      |Pull Request|Merged|#154|Update user guide: Add AntiVirus docs                                                                  |
|18.07.2019      |Pull Request|Merged|#155|PyPi docs: Add AntiVirus details                                                                       |
|19.07.2019      |Pull Request|Merged|#156|User docs: Add web deface detection docs                                                               |
|19.07.2019      |Pull Request|Merged|#157|PyPi docs: Add web deface details                                                                      |
|20.07.2019      |Pull Request|Merged|#169|Fix all contributors badge                                                                             |
|20.07.2019      |Pull Request|Merged|#170|User docs: Add IoT Anonymity Checker docs                                                              |
|20.07.2019      |Pull Request|Merged|#171|Update IoT checker args                                                                                |
|20.07.2019      |Pull Request|Merged|#172|PyPi docs: Add IoT checker docs                                                                        |
|20.07.2019      |Pull Request|Merged|#173|Update setup.py                                                                                        |
|20.07.2019      |Pull Request|Merged|#174|Dev docs: Update roadmap                                                                               |
|21.07.2019      |Pull Request|Merged|#175|Update developer docs                                                                                  |
|21.07.2019      |Pull Request|Merged|#176|Update setup.py for 1.5.1 release                                                                      |
|21.07.2019      |Pull Request|Merged|#177|User docs: Add OSINT feature details                                                                   |
|21.07.2019      |Pull Request|Merged|#178|PyPi: Add OSINT details                                                                                |
|                |            |      |    |                                                                                                       |
|**GSoC Phase - III**|            |      |    |                                                                                                       |
|23.07.2019      |Pull Request|Merged|#179|Elemental connection: Connect OSINT with Firewall                                                      |
|24.07.2019      |Pull Request|Merged|#180|Elemental connection: Connect server log monitor to OSINT                                              |
|24.07.2019      |Pull Request|Merged|#181|Elemental connection: Connect OSINT with IDS                                                           |
|24.07.2019      |Pull Request|Merged|#182|Elemental connection: Connect system log monitor with OSINT                                            |
|27.07.2019      |Pull Request|Merged|#183|Make Firewall smart: Learn bad IP address from IDS                                                     |
|28.07.2019      |Pull Request|Merged|#184|Make Firewall smart: Learn bad IP address from Real-time Server Log Monitor                            |
|28.07.2019      |Pull Request|Merged|#185|Make Firewall smart: Learn bad IP address from System log monitor                                      |
|28.07.2019      |Pull Request|Merged|#186|Fix contents spacing to improve readability and match the current doc formatting standards.            |
|29.07.2019      |Pull Request|Merged|#187|Feature: Introduce SecureTea server mode                                                               |
|1.08.2019       |Pull Request|Merged|#188|Feature: Introduce SecureTea System mode                                                               |
|1.08.2019       |Pull Request|Merged|#189|Dev docs: Add server mode details                                                                      |
|2.08.2019       |Pull Request|Merged|#190|Feature: Introduce SecureTea IoT mode                                                                  |
|2.08.2019       |Issue       |Closed|#191|Bug: Invalid Shodan API key blocks API Key attribute declaration                                       |
|2.08.2019       |Pull Request|Merged|#192|Fix #191: Bug: Invalid Shodan API key blocks API Key attribute declaration                             |
|2.08.2019       |Pull Request|Merged|#193|Dev docs: Add system mode details                                                                      |
|2.08.2019       |Issue       |Closed|#194|Bug: Setup failing to locate & copy OSINT files during installation                                    |
|4.08.2019       |Pull Request|Merged|#195|Fix #194: Identify OSINT as a python package                                                           |
|4.08.2019       |Issue       |Closed|#196|Bug: "pip install" fails to copy configuration file                                                    |
|4.08.2019       |Pull Request|Merged|#197|Fix #196: Instruct setup.py to copy configuration file                                                 |
|4.08.2019       |Pull Request|Merged|#198|Dev docs: Add IoT mode details                                                                         |
|4.08.2019       |Pull Request|Merged|#199|Make modes mutually exclusive                                                                          |
|5.08.2019       |Pull Request|Merged|#200|User docs: Add server mode details                                                                     |
|5.08.2019       |Pull Request|Merged|#201|PyPi docs: Add server mode details                                                                     |
|5.08.2019       |Issue       |Closed|#202|Bug: Failing to retrieve (KeyError) AntiVirus & Web Deface configurations from saved configuration file|
|5.08.2019       |Pull Request|Merged|#203|Fix #202: Look for appropriate keys                                                                    |
|6.08.2019       |Pull Request|Merged|#205|Feature: Add last login details to GUI dashboard                                                       |
|8.0.8.2019      |Pull Request|Merged|#206|GUI: Add Gmail notification text fields                                                                |
|7.08.2019       |Issue       |Closed|#207|Bug: Missing UTF-8 encoding definition                                                                 |
|7.08.2019       |Pull Request|Merged|#208|Fix #207 - Add missing UTF-8 module encoding definition                                                |
|9.08.2019       |Pull Request|Merged|#209|GUI: Add antivirus configuration fields                                                                |
|9.08.2019       |Pull Request|Merged|#210|Dev docs: Update roadmap                                                                               |
|10.08.2019      |Pull Request|Merged|#211|GUI: Add GUI configuration fields for Auto Server Patcher                                              |
|10.08.2019      |Pull Request|Merged|#212|Dev docs: Fix mode diagram missing link due to forked branch deletion                                  |
|10.08.2019      |Pull Request|Merged|#213|User docs: Add system mode details                                                                     |
|10.08.2019      |Pull Request|Merged|#214|PyPi docs: Add system mode details                                                                     |
|11..08.2019     |Pull Request|Merged|#215|GUI: Add GUI for system log monitor                                                                    |
|11..08.2019     |Pull Request|Merged|#216|User docs: Add IoT mode details                                                                        |
|11..08.2019     |Pull Request|Merged|#217|PyPi docs: Add IoT mode details                                                                        |
|14.08.2019      |Pull Request|Merged|#218|GUI: Add Firewall configuration fields                                                                 |
|14.08.2019      |Pull Request|Merged|#219|User docs: Provide support for technical jargon to improve user experience                             |
|14.08.2019      |Pull Request|Merged|#220|PyPi docs: Provide support for technical jargon to improve user experience                             |
|15.08.2019      |Pull Request|Merged|#221|GUI: Add server log monitor configuration fields                                                       |
|14.08.2019      |Pull Request|Merged|#222|Restructure README                                                                                     |
|15.08.2019      |Pull Request|Merged|#223|GUI: Add Intrusion Detection System configuration fields                                               |
|16.08.2019      |Pull Request|Merged|#225|GUI: Add Local Web Deface Detection & Prevention System                                                |
|16.08.2019      |Pull Request|Merged|#226|Collect network interface name before process division to avoid screen locking & base-10 error         |
|16.08.2019      |Pull Request|Merged|#227|Update README with the requested changes                                                               |
|17.08.2019      |Pull Request|Merged|#230|Fix #229 - Restore Python 2 support for input                                                          |
|17.08.2019      |Pull Request|Merged|#231|GUI: Add IoT Anonymity Checker & Insecure Headers configuration fields                                 |
|18.08.2019      |Pull Request|Merged|#232|End SSID spoof scanning loop when scanning not supported by the interface & safely log the message     |
|18.08.2019      |Pull Request|Merged|#233|Create guide for setting up local web serving over HTTPS                                               |
|19.08.2019      |Pull Request|Merged|#236|Re-structure, re-design and update the README.md                                                       |
|19.08.2019      |Pull Request|Merged|#238|Update user guide to latest                                                                            |
|19.08.2019      |Pull Request|Merged|#239|Update PyPi docs to latest                                                                             |
|22.08.2019      |Pull Request|Merged|#237|Update setup.py for v2.0 release                                                                       |
|23.08.2019      |Pull Request|Open|#240|Update README for v2.0 release                                                                           |

### Commits
View list of commits [here](https://github.com/OWASP/SecureTea-Project/commits?author=abhisharma404).

### Contribution graph and status

**Commits:**

![graph](/img/Commits_abhisharma404.png)

**Contribution to OWASP:**

![graph](/img/Contributions_abhisharma404.png)

## Blog posts made

- Blog: https://abhisharma404.blogspot.com/
- [GSoC 2019 with OWASP](https://abhisharma404.blogspot.com/2019/05/gsoc-2019-with-owasp.html)
- [Implementing a real-time server log monitoring](https://medium.com/@abhishekchem98/implementing-a-real-time-server-log-monitoring-a6c26607eb69)

## Screenshots screenscasts and tutorial videos

**Angular JS GUI dashboard**

![Last login dashboard](/img/dsh4.png)

![Configuration fields](/img/dsh7.png)

**Running Intrusion Detection System**

![Running IDS Recon](/img/ids_demo.gif)

![Running IDS R2L](/img/using_ids_mitm.gif)

**Running Anti Virus**

![Running AntiVirus](/img/using_antivirus.gif)

**Videos**

[Using SecureTea Web Deface Detection & Prevention System](https://www.youtube.com/watch?v=1vFaGxvzMh4)

## Future Work

The followings are the projected milestone for the next release:

- Testing project on various Linux flavours
- Peforming bug fixes
- Extending support to different Linux distributions
- Using SecureTea as a service instead of a Python package
- Packaging on `DEB` , `RPM` Linux packages

**Long roadmap:**

- Improving the current features

- Adding more features
    - **SecureTea browser plugin:** A plugin which can scan for harmful URL, monitor every URL, detect phishing sites & restrict internet activity.
    
    - **Real-time log visualization & monitoring dashboard:** If plotted in a graph with the right metrics, they can give back so vital information just by looking. And plotting them realtime? We are catching a thief red-handed, that’s quite cool! We can use Plotly to build this, it’s much more easy to integrate with a Flask app.
    
    - **Enhance AntiVirus:**
    
        **a. Behavioural based:<br>**
            i. Bring machine learning to detect and predict malware using Portable Executable(PE) headers.<br>
            ii. Analyze the behaviour of a file by looking at its API call, it’s hooks with the Kernel, it’s startup, system calls & TCP connections by using machine & deep learning.<br>
            iii. Convolutional neural networks (CNN) for malware visualization
            
        **b. Integrate volatility to perform m emory malware analysis:<br>**
            i. Catching memory malware is one of the toughest thing out there, catching it will advance our anti-virus even more.

## Personal experience and journey

Can't beleive it's been 8 months since I started contributing to OWASP Foundation. Time flies by so fast. I remember the first contribution I made to SecureTea-Project was a simple correction in the setup packaging & some readme typos. Since then I progressed to understand the code base at a more deeper level and started sending some core patches and that was it.

It's been an amazing journey so far. I can say my learning graph has shown an exponential growth. I have learned a lot during the last 3-4 months. I understood the importance of unit-tests and testing in general, understood that software is not only about coding, but a lot goes in maintaining a decent documentation and providing an intuitive version of software to the users for a satisfying user experience. Earlier, I considered tests as a waste of time and effort, instead tried to use that time to impelement a new feature or improve the current. I was wrong at many levels! As our codebase continued to grow, I understood testing keeps the code intact without you worrying about the regression when adding or a modifying a feature.

GSoC changed my view towards software engineering, following a certain prototype model, planning and discussing before implementing anything is crucial for a good software development. It's not only about coding instead regular testing, discussion with team members and regular beta releases are very important.

I personally learnt a lot from my mentor, [@rejahrehim](https://github.com/rejahrehim). He's been really supportive throughout the journey. The most important thing I learnt was keeping your calm and patience, and progressing with just one step at a time. I learned some good software development principles like maintaining a good commit history i.e. naming commits appropriately, which was something I overlooked every time. I'm really thankful of his support for all the techincal problems I faced midway.

The last month has been a quite hectic. My summer break ended and I had to manage my academics as well as achieve my GSoC milestones. I was running to maintain my 75% attendance and pulling up all nighters to complete my assignments xD. But finally, I was able to complete all my GSoC milestones :). Loads of thanks to my mentor for understanding and cooperating with the situations.

I would also like to thanks [@adeyosemanputra](https://github.com/adeyosemanputra). He's been like a brother through out the journey and taught me a lot. :)

## Conclusion

A great journey comes to an end! I'm very thankful to all the people who kept me motivated during this journey, be it my team members, friends and parents. I have met some amazing people and I have learnt a lot from them.

Though, GSoC comes to an end, I'll be actively contributing to open source and SecureTea Project.

<i>Keep calm and code</i>
