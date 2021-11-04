======================================================
Technical questions about the 2017 Equifax data breach
======================================================
`:star:`

  To go back to the main page about the 2017 Equifax data breach, click 
  `here`_.
  
`:warning:`

  **Disclaimer**

  This repository is for educational and informational purposes 
  only. The author, raul23, assumes no responsibility for the use 
  of this repository, code or any information contained therein. 
  The user is solely responsible for any action he/she takes with 
  this repository, code and information contained in it.

  Do not abuse this material. Be responsible.
  
.. contents:: **Contents**
   :depth: 4
   :local:
   :backlinks: top
   
`:information_source:`

  On February 10, 2020, the United States Department of Justice (DOJ) unsealed 
  an indictment charging four members of the Chinese People’s Liberation Army 
  (PLA) with hacking into the computer systems of the credit reporting agency 
  Equifax and stealing Americans’ personal data and Equifax’s valuable trade 
  secrets. [DOJ]_


How did the hackers allegedly hide their tracks?
================================================
According to the DOJ `indictment`_, the alleged four PLA hackers and their
co-conspirators supposedly hide their tracks when infiltrating Equifax's 
network by:

  1. using approximately thirty-four servers located in nearly twenty countries;
    
     [DOJ2]_ (paragraph 11, page 6)
  2. employing a variety of encrypted login protocols, including Remote Desktop 
     Protocol and Secure Shell software, which permitted them to connect to 
     servers over network connections from other servers they controlled; 
    
     [DOJ2]_ (paragraph 11, page 6)
  3. obtaining access to the servers located outside of China from reseller 
     hosting services; 
    
     [DOJ2]_ (paragraph 11, pages 6-7)
  4. using existing encrypted communication channels within Equifax's network to 
     send queries and commands, which allowed them to blend in with normal 
     network activity; 
    
     [DOJ2]_ (paragraph 12, page 7)
  5. compressing and dividing the data files so as to disguise the exfiltration 
     of sensitive personally identifiable information; 
    
     [DOJ2]_ (paragraph 12, page 7)
  6. deleting the compressed files after exfiltrating the sensitive data, and
  
     [DOJ2]_ (paragraph 13, page 7)
  7. configuring settings on at least one of their leased servers that wiped log 
     files on a daily basis in an effort to eliminate records of their activity.
    
     [DOJ2]_ (paragraph 13, page 7)

Web shells
==========
Definition of web shell
-----------------------
`:information_source:`

  A web shell [is] a script that can be uploaded to a web server to enable 
  remote administration of the server. A web shell can be used by an attacker 
  to gain access to functions on the server and to maintain persistent access 
  to a compromised server. [DOJ2]_

**Other definitions of web shell:**

1. A web shell is a shell-like interface that enables a web server to be 
   remotely accessed, often for the purposes of cyberattacks. 
   
   **Ref.:** `Wikipedia`_
2. A Web shell is a Web script that is placed on an openly accessible Web 
   server to allow an adversary to use the Web server as a gateway into a 
   network. A Web shell may provide a set of functions to execute or a 
   command-line interface on the system that hosts the Web server.
   
   **Adversaries may backdoor web servers with web shells to establish 
   persistent access to systems.** 
   
   **Ref.:** `MITRE`_
   
**Examples of web shells:**

- `China Chopper`_: 

    is a Web Shell hosted on Web servers to provide access 
    back into an enterprise network that does not rely on an infected system 
    calling back to a remote command and control server. It has been 
    used by several threat groups. [M]_
    
    It is approximately 4 kilobytes in size, first discovered in 2012. [W]_
  
- `SUPERNOVA`_: 

    is an in-memory web shell written in .NET C#. It was 
    discovered in November 2020 during the investigation of APT29's 
    SolarWinds cyber operation but determined to be unrelated. [M2]_

Example code of web shells
--------------------------
PHP
'''
JSP
'''

How web shells were allegedly used by the hackers?
--------------------------------------------------
`:information_source:`

  Also check `List of malicious files and web shells allegedly used by the 
  hackers`_ .
  
According to the DOJ `indictment`_, the alleged four PLA hackers and their
co-conspirators supposedly used web shells in various situations:

1. Once the web shells were installed to an Equifax web server, 
   reconnaissance of Equifax's online dispute portal started.
   
   [DOJ2]_ (paragraph 8, page 5)
   
2. Web shells (created through Apache Struts) were used to interact with 
   Equifax's back-end databases.
  
   [DOJ2]_ (paragraph 8, page 5)
   
3. Web shells (created through Apache Struts) in combination with Apache 
   Struts commands and SQL commands were used to review database records 
   in small segments.
   
   [DOJ2]_ (paragraph 14.b, page 8)

References
==========
.. [DOJ] “Press Release: Chinese Military Personnel Charged with Computer Fraud, 
   Economic Espionage and Wire 
   Fraud for Hacking into Credit Reporting Agency Equifax.” *The United States 
   Department of Justice*, 10 Feb. 2020,
   https://www.justice.gov/opa/pr/chinese-military-personnel-charged-computer-fraud-economic-espionage-and-wire-fraud-hacking.
   `Archived <https://archive.md/JtDCY>`__.
   
.. [DOJ2] “Criminal Indictment: UNITED STATES OF AMERICA *v.* WU ZHIYONG, WANG 
   QIAN, XUKE, LIU LEI” *The United States Department of Justice*, 28 Jan. 
   2020, https://www.justice.gov/opa/press-release/file/1246891/download (PDF).
   `Archived <https://web.archive.org/web/20210702191105/https://www.justice.gov/opa/press-release/file/1246891/download>`__.

.. [M ] “Server Software Component: Web Shell.” *Server Software Component: 
   Web Shell, Sub-Technique T1505.003 - Enterprise | MITRE ATT&CK®*, 
   26 July 2021,
   https://attack.mitre.org/techniques/T1505/003/.
   `Archived <https://archive.md/WpePx>`_.
   
.. [M] “China Chopper.” *Software S0020 | MITRE ATT&CK®*, 
   17 Oct. 2021,
   https://attack.mitre.org/software/S0020/.
   `Archived <https://archive.md/dox4Z>`__.
   
.. [M2] “SUPERNOVA.” *Software S0578 | MITRE ATT&CK®*, 
   https://attack.mitre.org/software/S0578/.
   `Archived <https://archive.md/vRJc7>`__.
   
.. [W] “China Chopper.” *Wikipedia*, Wikimedia Foundation, 
   16 Mar. 2021, https://en.wikipedia.org/wiki/China_Chopper.

.. [W ] “Web Shell.” *Wikipedia*, Wikimedia Foundation, 
   21 July 2021, https://en.wikipedia.org/wiki/Web_shell.

.. URLs
.. _China Chopper: https://attack.mitre.org/software/S0020/
.. _here: https://github.com/raul23/equifax-data-breach/blob/main/README.rst
.. _indictment: https://www.justice.gov/opa/press-release/file/1246891/download
.. _List of malicious files and web shells allegedly used by the hackers: ./list_of_malicious_files.rst
.. _MITRE: https://attack.mitre.org/techniques/T1505/003/
.. _SUPERNOVA: https://attack.mitre.org/software/S0578/
.. _Wikipedia: https://en.wikipedia.org/wiki/Web_shell
