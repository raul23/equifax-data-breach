=============================
Other interesting information
=============================
`:star:`

  To go back to the main page about the 2017 Equifax data breach, click 
  `here`_.
  
----------

- Why is patching the security hole (`CVE-2017-5638`_) considered as labor 
  intensive and difficult?

     ... in part because it involved downloading an updated version of Struts 
     and then using it to rebuild all apps that used older, buggy Struts versions. 
     Some websites may depend on dozens or even hundreds of such apps, which may 
     be scattered across dozens of servers on multiple continents. Once rebuilt, 
     the apps must be extensively tested before going into production to ensure 
     they don't break key functions on the site. [G]_

- `Apache Struts`_ is used across the Fortune 100 to provide web applications 
  in Java, and it powers front- and back-end applications, including Equifax's 
  public website. [W]_
  
- `Equifax Lawsuit: ‘Admin’ As Password At Time Of 2017 Breach`_

    According to the `filing`_ in the U.S. District Court for the Northern 
    District of Georgia, Atlanta Division, Equifax was protecting sensitive 
    personal information on a portal used to manage credit disputes with the 
    username “admin.”   
    
    And if that wasn’t enough, the password protecting that data was probably 
    the first one an attacker would guess: Yes that’s right, it was also 
    “admin,” according to the lawsuit.
    
    The lawsuit also points out that Equifax was storing unencrypted user data 
    on a public facing server–so it could have been viewed by any attacker who 
    chose to compromise it. Meanwhile, Equifax didn’t encrypt its mobile 
    applications either–and when it did encrypt data, it left the encryption 
    keys on the same public facing servers.
    
  .. raw:: html

     <div align="center">
     <a href="https://www.dictionary.com/e/wp-content/uploads/2020/05/picard-facepalm.jpg">
     <img src="https://www.dictionary.com/e/wp-content/uploads/2020/05/picard-facepalm.jpg" style="width:500px;height:300px;"/>
     </a>
     </div>
     
- **Equifax Former CIO Jailed For Insider Trading:**

    In the summer of 2019, Jun Ying, the former `Chief Information Officer CIO of 
    Equifax was sentenced to four months`_ in a federal prison for insider 
    trading.
    
    Ying had sold off his stock options before the 2017 data breach became public 
    knowledge.
    
  **Ref.:** `Silicon.co.uk`_
 
- The US officials said that it was important to name the four PLA members 
  because according to them it will help to publicly shame them. But it is 
  doubtful if the DOJ indictment will make them feel shame for what they did 
  to millions of people. If they were receiving orders from higher up in the 
  Chinese army, then the PLA would support them and make sure they are being 
  treated well by their comrades for getting away with important PII from 
  millions of americans in one of the most important data breaches (we are 
  talking about a credit monitoring company that collects tremendous amount of 
  information about lots of people in the US and around the world). The Chinese 
  army would surely be happy to use these PII in whatever secret projects they 
  might be working on.

    None of them are in custody, nor are they likely to be any time soon. But 
    officials said that charging and naming them served the purpose of 
    **publicly shaming** them for their actions and enabled the United States 
    to arrest them if they travel one day. [F]_

References
==========
.. [F] Fifield, Anna. “China Rebuffs U.S. Charges of Cyberespionage over Equifax 
   Hack.” *The Washington Post*, WP Company, 20 Feb. 2020, 
   https://www.washingtonpost.com/world/asia_pacific/china-rebuffs-american-charges-of-cyber-espionage-over-equifax-hack/2020/02/11/b95fd932-4ca2-11ea-967b-e074d302c7d4_story.html.
   `Archived <https://archive.md/W7b4b>`__.
   
.. [G] Goodin, Dan. “Failure to Patch Two-Month-Old Bug Led to Massive Equifax 
   Breach.” *Ars Technica*, 13 Sept. 2017, 
   https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/.
   `Archived <https://archive.md/https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/>`__.

.. [W] Whittaker, Zack. “Equifax Confirms Apache Struts Flaw It Failed to Patch 
   Was to Blame for Data Breach.” *ZDNet*, 13 Sept. 2017, 
   https://www.zdnet.com/article/equifax-confirms-apache-struts-flaw-it-failed-to-patch-was-to-blame-for-data-breach/.
   `Archived <https://archive.md/Qxreg>`__.

.. URLs
.. _Apache Struts:
.. _Chief Information Officer CIO of Equifax was sentenced to four months:
.. _CVE-2017-5638:
.. _Equifax Lawsuit\: ‘Admin’ As Password At Time Of 2017 Breach:
.. _filing:
.. _here: https://github.com/raul23/equifax-data-breach/blob/main/README.rst
.. _Silicon.co.uk: 
