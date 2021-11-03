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

How did the hackers allegedly hide their tracks?
================================================
TODO

How web shells were allegedly used by the hackers?
==================================================
Definition of web shell
-----------------------
`:information_source:`

  A web shell [is] a script that can be uploaded to a web server to enable 
  remote administration of the server. A web shell can be used by an attacker 
  to gain access to functions on the server and to maintain persistent access 
  to a compromised server. [DOJ]_

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

References
==========
.. [DOJ] “Criminal Indictment: UNITED STATES OF AMERICA *v.* WU ZHIYONG, WANG 
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
.. _here: ./README.rst
.. _indictment: https://www.justice.gov/opa/press-release/file/1246891/download
.. _MITRE: https://attack.mitre.org/techniques/T1505/003/
.. _SUPERNOVA: https://attack.mitre.org/software/S0578/
.. _Wikipedia: https://en.wikipedia.org/wiki/Web_shell
