========================
2017 Equifax data breach
========================

.. raw:: html

   <div align="center">
   <img src="https://www.omegawealthmanagement.com/wp-content/uploads/2020/01/equifax.jpg" style="width:550px;height:250px;"/>
   <p><b><a href="https://www.omegawealthmanagement.com/were-you-affected-by-the-equifax-data-breach-in-2017/">Reference</a></b></p>
   </div>

.. contents:: **Contents**
   :depth: 4
   :local:
   :backlinks: top

`:information_source:`

  On September 7, 2017, Equifax, one of the largest credit reporting agencies in America, 
  announced that an unauthorized third party gained access to Equifax data on as many as 
  143 million Americans. [M]_
  
  The number of affected people is roughly half of the US population of 323 million. [N2]_
  
`:warning:`

  Equifax learned about the breach on July 29 but didn't reveal it for more than a month. [N2]_

Some important information
========================
- On March 9, 2017, the company's IT team was informed of a vulnerability affecting the `Apache 
  Struts software`_ it used on its dispute resolution portal, with instructions to patch it 
  in 48 hours. That didn't happen. [H]_
- On May 13, 2017, the attackers hit the jackpot with Equifax's dispute portal, where 
  people could go to argue about claims. [N]_
- The breach was discovered on `29 July 2017`_. [M]_
- On September 7, 2017, Equifax, one of the largest credit reporting agencies in America, 
  announced that an unauthorized third party gained access to Equifax data on as many as 
  143 million Americans. [M]_
- As a result, the `CEO`_, `CIO and CSO`_ had to go. [T]_
- In both October 2017 [WE]_ and March 2018 [MM]_, Equifax reported that an additional 2.5 and 2.4 million 
  American consumer records were accessed, respectively, bringing the total to 147.9 million. [WK]_

What kinds of data were accessed?
========================
- The information accessed primarily includes names, Social Security numbers, birth dates, 
  addresses and, in some instances, driver's license numbers. [E]_
  
  The driver's license data of around 10.9 million Americans were compromised. [CM]_

- In addition, credit card numbers for approximately 209,000 U.S. consumers, and certain 
  dispute documents with personal identifying information for approximately 182,000 U.S. 
  consumers, were accessed. [E]_
  
- Equifax also identified unauthorized access to limited personal information for certain 
  UK and Canadian residents. [E]_
  
  Information on an estimated range of under 400,000 up to 44 million British residents. [BBC]_ [HA]_ 
  
  The company said that 8,000 Canadian citizens were impacted. [S]_
  
  An additional 11,670 Canadians were affected as well, later revealed by Equifax. [WK]_ [C]_

How was the data breached?
========================
`:information_source:`

  On 7 September 2018, US lawmakers released a report (`PDF`_ and `archive`_) detailing exactly how the 
  credit-monitoring company was hacked.
  
  The report comes from the Government Accountability Office (GAO), the agency that provides 
  auditing and investigative services for Congess.
  
  **Ref.:** `cnet.com 
  <https://www.cnet.com/tech/services-and-software/equifaxs-hack-one-year-later-a-look-back-at-how-it-happened-and-whats-changed/>`__

By exploiting a vulnerability on one of the company's U.S.-based web servers. [M]_

It seems that the underlying legacy codebase that handled the [Equifax] web application 
was vulnerable enough for an attacker to exploit. [M]_

1. Hackers used an Apache Struts vulnerability (`CVE-2017-5638`_), `a months-old issue that Equifax knew about but failed to fix`_, 
   and gained access to internal login credentials (for Equifax employees) for three servers. Those credentials allowed them to access 
   48 credit monitoring databases containing personal information. [N]_ [T]_
2. They searched the databases about 9,000 times for sensitive personal information while hiding the searches through encryption. [B]_
3. They stuffed the personal information in temporary files, compressed them and divided them into smaller-sized files to 
   increase their chances of transmitting the stolen data without being noticed. [B]_ [N]_
4. They used 34 servers in 20 countries during the breach and employed various other techniques, 
   such as remote-desktop access and encrypted log-ins, to mask the origin of the hack. [B]_
5. They deleted the compressed files after transferring the data into external storage, 
   then configured settings to wipe out information tracking their activity. [B]_
6. The thieves spent 76 days within Equifax's network before they were detected. [N]_

`:information_source:`

  While the failure to update Struts was a key failure, analysis of the breach found further faults in Equifax' 
  system that made it easy for the breach to occur, including [WK]_:
  
  - the insecure network design which lacked sufficient segmentation [NL]_
  - potentially inadequate encryption of personally identifiable information (PII) [GS]_, and
  - ineffective breach detection mechanisms. [L]_

.. raw:: html

   <div align="center">
   <img src="https://camo.githubusercontent.com/4dbe1733c0ea00a63c6096fef006392d8544b2ef9e8947f3aafca507ba7837a1/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f313430302f302a46334476476b37755234583538613566" style="width:700px;height:500px;"/>
   <p><b>A chart from the <a href="https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf">GAO report</a>
      describing how Equifax was breached.</b></p>
   </div>
   
The US says members of the Chinese military hacked Equifax
==========================================================
`:warning:`

  The United States Department of Justice (DOJ) is very careful not to imply that the Chinese army is 
  directly responsible for the data breach.
  Thus, the `DOJ indictment`_ and their `press release`_ target specifically members of the Chinese 
  People’s Liberation Army (PLA); more precisely they are part of PLA’s 54th Research Institute, a component 
  of the Chinese military.
  
  The majority of mainstream news sites are also careful in their titles so as 
  to be specific in who are being accused by the DOJ:
  
  - `Chinese Military Hackers Charged in Equifax Breach`_ (FBI News)
  - `Chinese Military Officers Hacked Equifax, Justice Department Say`_ (Defense One)
  - `Equifax: US charges four Chinese military officers over huge hack`_ (BBC News)
  - `Four Members of China's Military Indicted for Massive Equifax Breach`_ (The Wall Street Journal)
  - `Justice Department charges 4 members of Chinese military for massive Equifax hack`_ (CBS NEWS)
  - `U.S. Charges Chinese Military Officers in 2017 Equifax Hacking`_ (The New York Times)
  
  Though you still have some news articles with titles implying that it is the whole
  Chinese army that is being targeted by the DOJ:

  - `What is the PLA, and why do feds believe they hacked Equifax?`_ (The Atlanta Journal-Constitution)
  - `The US says the Chinese military hacked Equifax. Here’s how.`_ (MIT Technology Review)

The US indictment
-----------------
On February 10, 2020, the DOJ indicted four members of 
China's military on nine charges related to the hack. [DOJ]_

From the DOJ's press release about the `indictment`_ 
(`archive <https://web.archive.org/web/20210725031951/https://www.justice.gov/opa/press-release/file/1246891/download>`__) 
of the four Chinese military members [DOJ]_:

  The nine-count indictment alleges that Wu Zhiyong (吴志勇), Wang Qian (王乾), Xu Ke (许可) and Liu Lei 
  (刘磊) were members of the PLA’s 54th Research Institute, a component of the Chinese military.  They 
  allegedly conspired with each other to hack into Equifax’s computer networks, maintain unauthorized 
  access to those computers, and steal sensitive, personally identifiable information of 
  approximately 145 million American victims. 

DOJ evidence that China's military personnel are behind the Equifax data breach
-------------------------------------------------------------------------------
`:information_source:`

  These are evidence that I was able to gather from the DOJ `indictment`_. 
  
  **TODO:** gather evidence from other governmental sources
  
1. Multiple China-based IP addresses were allegedly accessed during the intrusion by the conspirators:

   - The majority of the 9000 SQL queries [to the credit monitoring databases] were issued by conspirators using two
     **China-based IP addresses** that connected directly to Equifax' s network. []_ page 6, paragraph 9
     
     **NOTE:** the indictment doesn't name these two **China-based IP addresses** like in other places
     of the document (e.g. China Server #1)
   - **China Server #1:** On or about June 16, 2017, a conspirator using a China-based IP address ("China Server #1"), 
     which was repeatedly accessed during the intrusion by WANG QIAN, logged into a Taiwanese IP 
     address ("the Taiwan Server") via Remote Desktop Protocol software and copied the 
     malicious file "jndi. txt." []_ page 8, paragraph e
   - **China Server #2:** On or about the same day [of July 7, 2017], another China-based IP address 
     ("China Server #2"), which was also repeatedly accessed during the intrusion by WANG QIAN, exploited 
     the Apache Struts vulnerability on Equifax' s online dispute portal. 
   - **China Server #3:** On or about the same day and July 9, 2017, XUKE used a 
     different China-based IP address ("China Server #3") to conduct reconnaissance on Equifax' s online dispute portal. 
   - **China Server #4:** On or about July 10, 2017, a conspirator using another China-based IP address 
     ("China Server #4") logged into the Taiwan Server and copied the malicious file "abc.txt" to the Taiwan Server.
   - **China Server #5:** On or about July 10, 2017, a conspirator using another China-based IP address ("China Server #5'') then utilized
     the malicious web shell ''css.jsp," which was previously installed on Equifax' s network, to issue a command 
     to download the "abc. txt" file from the Taiwan Server.
   - **China Server #6:** On or about the same day [of July 10, 2017], a conspirator who was logged into another China-based IP address 
     ("China Server #6") utilized the malicious web shell ''boxover.jsp" to query an Equifax database 
     table and store the results in output files.
   
   `:information_source:`
   
     Reading the `indictment`_, you have the impression that the US authorities were somehow able to 
     exactly pinpoint who among the four members of the PLA logged to Equifax's network at a particular time of the day.
     
     However for some other days of the attack, the US investigators lose their special talent to exactly identify 
     who is logging into Equifax's network and instead used the word "conspirator".
   
   `:information_source:`
     
     The conspirators also allegedly accessed IP addresses from locations outside of China:
     
     - Switzerland, []_ page 9, paragraph f
     - Taiwan, []_ pages 10 paragraph I
     - Singapore, []_ page 11 paragraphs o, q

Weak evidence
-------------
The evidence gathered from the DOJ `indictment`_ is very weak to support the claim that 
the four members of the PLA were the perpretrators of the Equifax data breach.
  
- No much information is given about the four PLA members: Wu Zhiyong (吴志勇), Wang Qian (王乾), 
  Xu Ke (许可) and Liu Lei (刘磊).
  
  The DOJ `indictment`_, their press release and mainstream news articles only provide their
  names and pictures. Even their `FBI most wanted`_ poster only give their names.
  
  How old are they? What are their ranks in the Chinese military? Were they receiving orders
  from higher up or were they acting on their own? Where are those pictures provided in the
  indictment of three of the four PLA members coming from? 
  
  .. raw:: html

     <div align="center">
     <img src="https://www.cnet.com/a/img/uf_P-IUAQf-_-47zXmpuSWcyqs8=/940x0/2020/02/10/489560f1-9731-4957-af0d-9b0a947da334/screen-shot-2020-02-10-at-10-18-15-am.png" style="width:700px;height:400px;"/>
     <p><b>In the news articles and the DOJ <a href="https://www.justice.gov/opa/press-release/file/1246891/download">indictment</a>, they don't provide a picture for the alleged PLA member Liu Lei.
        However in the <a href="https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute">FBI poster</a>, 
        you get all four pictures (though <a href="https://archive.md/3qA8b">at first</a> the FBI also only shown three pics). Very odd that the DOJ worked for 2 years investigating the Equifax data breach
        and could not get a picture for Liu Lei to include in their indictment.</b></p>
     </div>
  
  .. raw:: html

     <div align="center">
     <img src="https://www.fbi.gov/@@dvpdffiles/8/c/8c0b4ce2b3c9448b95b13f19a89fc658/normal/dump_1.gif"/>
     <p><b>PLA members wanted by the
       <a href="https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute">FBI</a>.</b></p>
     </div>

- There is no explanation in the `indictment`_ how the US authorities came to the
  conclusion that the four named PLA members were directly related to the network intrusions.

- Some of the evidence is based on multiple IP addresses allegedly originating from China.

  It seems very sloppy for the four members of the PLA to allegedly log 
  multiple times into Equifax's systems directly from Chinese-based IP addresses. These conspirators
  are not your average Joe that doesn't know much about network forensics but are supposedly part of 
  PLA's 54th Research Institute which has traditionally focused on supporting electronic 
  warfare akin to Cyber Command as opposed to cyber espionage [VD]_. 
  
  Therefore, these four accused members of the PLA should know very well how to hide their tracks and use
  only IP addresses from outside China. 
  
- Since it is extremely unlikely for the DOJ to arrest the four PLA members, the indictment can
  be very poor in the quality of the evidence. The case will not go in front of 
  a judge and jury where the evidence presented by the prosecutors would have been scrutinized.
  
  Thus, the DOJ is not incentivized to gather solid evidence that could link the four PLA members
  to the Equifax data breach:
  
    Officials acknowledged they were unlikely to face prosecution in a U.S. courtroom. [V]_ 
  
Reading the many mainstream news articles (even outside USA like UK and Canada), you get the 
feeling that everyone just went along with the narrative of the DOJ 
that four PLA members are responsible for the Equifax data breach.

However, `RT`_ is among the only news sites that questioned the link between the four
PLA members and the data breach as promulgated by the DOJ:

  It remains unclear how the DOJ concluded that four members of the Chinese military were 
  responsible, whether they were supposedly acting on their own or on state orders, or how 
  it intends to bring them to a US court. 
  
Equifax data breach by the numbers
==================================
.. raw:: html

   <div align="center">
   <img src="https://ei.marketwatch.com/Multimedia/2018/09/07/Photos/NS/MW-GP711_equifa_20180907130002_NS.jpg" style="width:300px;height:400px;"/>
   <p><b>Chart from 
      <a href="https://www.marketwatch.com/story/the-equifax-data-breach-in-one-chart-2018-09-07">marketwatch.com</a></b></p>
   </div>
   
.. raw:: html

   <div align="center">
   <img src="https://www.alliedsolutions.net/-/media/alliedwww/images/equifax_infographic_r5_777x450.ashx" style="width:500px;height:400px;"/>
   <p><b>Chart from 
      <a href="https://www.alliedsolutions.net/resources/allied-insights/2017/10/03/3-ways-to-manage-equifax-breach">alliedsolutions.net</a></b></p>
   </div>
   
.. raw:: html

   <div align="center">
   <img src="https://i.insider.com/59b2f0fb45e2384d338b4576" style="width:500px;height:400px;"/>
   <p><b>Chart from 
      <a href="https://www.businessinsider.com/how-equifax-compares-to-biggest-hacks-of-all-time-chart-2017-9">businessinsider.com</a></b></p>
   </div>   

   
Other interesting information
=============================
- As Ars warned in March of 2017, patching the security hole (`CVE-2017-5638`_) 
  was labor intensive and difficult, in part because it involved downloading an 
  updated version of Struts and then using it to rebuild all apps that used 
  older, buggy Struts versions. Some websites may depend on dozens or even 
  hundreds of such apps, which may be scattered across dozens of servers on 
  multiple continents. Once rebuilt, the apps must be extensively tested before 
  going into production to ensure they don't break key functions on the site. 
  [G]_

- `Apache Struts`_ is used across the Fortune 100 to provide web applications in 
  Java, and it powers front- and back-end applications, including Equifax's 
  public website. [W]_
 
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
    **publicly shaming** them for their actions and enabled the United States to 
    arrest them if they travel one day. [FA]_

Links
=====
`:information_source:`

  The links are listed in chronological order starting from oldest.

- `“Vulnerability Details : CVE-2017-5638.” 
  <https://www.cvedetails.com/cve/CVE-2017-5638/>`__ *CVE*, 11 March 2017. 
  `Archived <https://archive.md/IKpS5>`__.
  
- Inc., Equifax. `“Equifax Announces Cybersecurity Incident Involving Consumer 
  Information.“ 
  <https://www.prnewswire.com/news-releases/equifax-announces-cybersecurity-incident-involving-consumer-information-300515960.html>`__ 
  *PrNewsWire*, 7 Sept. 2017. `Archived <https://archive.md/MBXzP>`__.
  
- Mathews, Lee. `“Equifax Data Breach Impacts 143 Million Americans.” 
  <https://www.forbes.com/sites/leemathews/2017/09/07/equifax-data-breach-impacts-143-million-americans/?sh=16bb95ef356f>`__ 
  *Forbes*, Forbes Magazine, 7 Sept. 2017. 
  `Archived <https://archive.md/fo2um>`__.

- Haselton, Todd. `“Credit Reporting Firm Equifax Says Data Breach Could 
  Potentially Affect 143 Million US Consumers.” 
  <https://www.cnbc.com/2017/09/07/credit-reporting-firm-equifax-says-cybersecurity-incident-could-potentially-affect-143-million-us-consumers.html>`__
  *CNBC*, 8 Sept. 2017.
  `Archived 
  <https://archive.md/https://www.cnbc.com/2017/09/07/credit-reporting-firm-equifax-says-cybersecurity-incident-could-potentially-affect-143-million-us-consumers.html>`__.
  
- Hern, Alex. `“Equifax Told to Inform Britons Whether They Are at Risk after 
  Data Breach.” 
  <https://www.theguardian.com/technology/2017/sep/08/equifax-told-to-inform-britons-whether-they-are-at-risk-after-data-breach>`__ 
  *The Guardian*, Guardian News and Media, 8 Sept. 2017. 
  `Archived <https://archive.md/a3PmP>`__.

- Lomas, Natasha. `“Equifax Breach Disclosure Would Have Failed Europe's Tough 
  New Rules.” 
  <https://techcrunch.com/2017/09/08/equifax-breach-disclosure-would-have-failed-europes-tough-new-rules/>`__
  *TechCrunch*, 8 Sept. 2017. `Archived <https://archive.md/ZtPUF>`__.
  
- Ng, Alfred, and Musil, Steven. `“Equifax Data Leak May Affect Nearly Half the 
  US Population.” 
  <https://www.cnet.com/tech/services-and-software/equifax-data-leak-hits-nearly-half-of-the-us-population/>`__ 
  *CNET*, 8 Sept. 2017. `Archived <https://archive.md/dH7ei>`__.

- Newman, Lily Hay. `“How to Stop the Next Equifax-Style Megabreach-Or At Least 
  Slow It Down.” <https://www.wired.com/story/how-to-stop-breaches-equifax/>`_ 
  *Wired*, Conde Nast, 12 Sept. 2017. `Archived <https://archive.md/xL7vb>`__.
  
- Goodin, Dan. `“Failure to Patch Two-Month-Old Bug Led to Massive Equifax Breach.” 
  <https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/>`__ 
  *Ars Technica*, 13 Sept. 2017.
  `Archived 
  <https://archive.md/https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/>`__.

- Gallagher, Sean. `“Equifax Hackers Stole Data for 200k Credit Cards from 
  Transaction History.” 
  <https://arstechnica.com/information-technology/2017/09/equifax-hackers-stole-data-for-200k-credit-cards-from-transaction-history/>`__ 
  *Ars Technica*, 14 Sept. 2017. `Archived <https://archive.md/5Bkbc>`__.

- Whittaker, Zack. `“Equifax Confirms Apache Struts Flaw It Failed to Patch Was 
  to Blame for Data Breach.” 
  <https://www.zdnet.com/article/equifax-confirms-apache-struts-flaw-it-failed-to-patch-was-to-blame-for-data-breach/>`__
  *ZDNet*, 14 Sept. 2017. `Archived <https://archive.md/Qxreg>`__.
  
- `“Equifax Says Almost 400,000 Britons Hit in Data Breach.” 
  <https://www.bbc.com/news/technology-41286638>`__ *BBC News*, BBC, 15 Sept. 
  2017. `Archived <https://archive.md/zpbLF>`__.

- Hautala, Laura. `“Equifax Ex-CEO: 'Both Human Error and Tech Failures' in 
  Massive Data Breach.” 
  <https://www.cnet.com/tech/services-and-software/equifax-ceo-data-breach-heres-what-went-wrong/>`_ 
  *CNET*, 2 Oct. 2017. `Archived <https://archive.md/CuNmM>`__.
  
- Shepardson, David. `“Equifax Failed to Patch Security Vulnerability in March: 
  Former CEO.” 
  <https://www.reuters.com/article/us-equifax-breach/equifax-failed-to-patch-security-vulnerability-in-march-former-ceo-idUSKCN1C71VY>`__ 
  *Reuters*, Thomson Reuters, 2 Oct. 2017. `Archived <https://archive.md/MJ7zq>`__.
  
- Weise, Elizabeth, and Nathan Bomey. `“Equifax Breach Hit 2.5 Million More 
  Americans than First Believed.” 
  <https://www.usatoday.com/story/tech/2017/10/02/equifax-breach-hit-2-5-million-more-americans-than-first-believed/725100001/>`__ 
  *USA Today*, Gannett Satellite Information Network, 2 Oct. 2017. 
  `Archived <https://archive.md/TfhLK>`__.

- Chin, Monica. `“On Top of Everything Else, Equifax Hackers Got 10 Million 
  Driver's Licenses.” 
  <https://mashable.com/article/equifax-hackers-got-drivers-licenses.>`__
  *Mashable*, 11 Oct. 2017. `Archived <https://archive.md/ubD10>`__.

- `“Equifax Doubles Number of Canadians Hit by Breach, Now More than 19,000 | 
  CBC News.” 
  <https://www.cbc.ca/news/business/equifax-canadians-affected-update-1.4424066>`__ 
  *CBCnews*, CBC/Radio Canada, 28 Nov. 2017. `Archived <https://archive.md/FpI1t>`__.
  
- Ng, Alfred. `“How the Equifax Hack Happened, and What Still Needs to Be Done.” 
  <https://www.cnet.com/tech/services-and-software/equifaxs-hack-one-year-later-a-look-back-at-how-it-happened-and-whats-changed/>`__ 
  *CNET*, 7 Sept. 2018. `Archived <https://archive.md/NVeDV>`__.

- Berr, Jonathan. `“Equifax Breach Exposed Data for 143 Million Consumers.” 
  <https://www.cbsnews.com/news/equifax-breach-exposes-data-for-143-million-consumers/>`__
  *CBS News*, CBS Interactive, 8 Apr. 2018. `Archived 
  <https://archive.md/u7r1U>`__.

- Bomey, Nathan. `“How Chinese Military Hackers Allegedly Pulled off the Equifax Data Breach, Stealing Data from 145 Million Americans.” 
  <https://www.usatoday.com/story/tech/2020/02/10/2017-equifax-data-breach-chinese-military-hack/4712788002/>`__
  *USA Today*, Gannett Satellite Information Network, 10 Feb. 2020.
  `Archived <https://archive.md/tMyN3>`__.

- Viswanatha, Aruna, et al. `“Four Members of China's Military Indicted Over 
  Massive Equifax Breach.” 
  <https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824>`__ 
  *The Wall Street Journal*, Dow Jones & Company, 11 Feb. 2020.
  `Archived <https://archive.md/JDvB1>`__.

- `“Press Release: Chinese Military Personnel Charged with Computer Fraud, 
  Economic Espionage and Wire Fraud for Hacking into Credit Reporting Agency 
  Equifax.” 
  <https://www.justice.gov/opa/pr/chinese-military-personnel-charged-computer-fraud-economic-espionage-and-wire-fraud-hacking>`__
  *The United States Department of Justice*, 13 Feb. 2020.
  `Archived <https://archive.md/JtDCY>`__. 
  
- Fifield, Anna. `“China Rebuffs U.S. Charges of Cyberespionage over Equifax 
  Hack.” 
  <https://www.washingtonpost.com/world/asia_pacific/china-rebuffs-american-charges-of-cyber-espionage-over-equifax-hack/2020/02/11/b95fd932-4ca2-11ea-967b-e074d302c7d4_story.html>`__ 
  *The Washington Post*, WP Company, 20 Feb. 2020. 
  `Archived <https://archive.md/W7b4b>`__.
  
- “2017 Equifax Data Breach.” *Wikipedia*, Wikimedia Foundation, 25 Oct. 2021, 
  https://en.wikipedia.org/wiki/2017_Equifax_data_breach.

- `“Equifax Data Breach Lawsuit.” 
  <https://www.forthepeople.com/class-action-lawyers/equifax-data-breach-lawsuit/>`__ 
  *Morgan & Morgan*. `Archived <https://archive.md/GRPq3>`__.
  
- Turcsányi, Gergő. `“Deep Dive into the Equifax Breach and the Apache Struts 
  Vulnerability.” 
  <https://avatao.com/blog-deep-dive-into-the-equifax-breach-and-the-apache-struts-vulnerability/>`__ 
  *Avatao*. `Archived <https://archive.md/LPy4G>`__.

References
==========
.. [B] Bomey, Nathan. “How Chinese Military Hackers Allegedly Pulled off the 
   Equifax Data Breach, Stealing Data from 145 Million Americans.” *USA Today*, 
   Gannett Satellite Information Network, 10 Feb. 2020, 
   https://www.usatoday.com/story/tech/2020/02/10/2017-equifax-data-breach-chinese-military-hack/4712788002/.
   `Archived <https://archive.md/tMyN3>`__.
   
.. [BBC] “Equifax Says Almost 400,000 Britons Hit in Data Breach.” *BBC News*, 
   BBC, 15 Sept. 2017, https://www.bbc.com/news/technology-41286638.
   `Archived <https://archive.md/zpbLF>`__.
   
.. [C] “Equifax Doubles Number of Canadians Hit by Breach, Now More than 19,000 
   | CBC News.” *CBCnews*, CBC/Radio Canada, 28 Nov. 2017, 
   https://www.cbc.ca/news/business/equifax-canadians-affected-update-1.4424066.
   `Archived <https://archive.md/FpI1t>`__.
   
.. [CM] Chin, Monica. “On Top of Everything Else, Equifax Hackers Got 10 Million Driver's Licenses.” 
   *Mashable*, 11 Oct. 2017, https://mashable.com/article/equifax-hackers-got-drivers-licenses.
   `Archived <https://archive.md/ubD10>`__.
   
.. [DOJ] “Press Release: Chinese Military Personnel Charged with Computer Fraud, Economic Espionage and Wire 
   Fraud for Hacking into Credit Reporting Agency Equifax.” *The United States Department of Justice*, 13 Feb. 2020,
   https://www.justice.gov/opa/pr/chinese-military-personnel-charged-computer-fraud-economic-espionage-and-wire-fraud-hacking.
   `Archived <https://archive.md/JtDCY>`__.

.. [E] Inc., Equifax. “Equifax Announces Cybersecurity Incident Involving Consumer Information.“ *PrNewsWire*, 7 Sept. 2017, 
   https://www.prnewswire.com/news-releases/equifax-announces-cybersecurity-incident-involving-consumer-information-300515960.html.
   `Archived <https://archive.md/MBXzP>`__.

.. [FA] Fifield, Anna. “China Rebuffs U.S. Charges of Cyberespionage over Equifax Hack.” 
   *The Washington Post*, WP Company, 20 Feb. 2020, 
   https://www.washingtonpost.com/world/asia_pacific/china-rebuffs-american-charges-of-cyber-espionage-over-equifax-hack/2020/02/11/b95fd932-4ca2-11ea-967b-e074d302c7d4_story.html.
   `Archived <https://archive.md/W7b4b>`__.

.. [G] Goodin, Dan. “Failure to Patch Two-Month-Old Bug Led to Massive Equifax Breach.” *Ars Technica*, 13 Sept. 2017, 
   https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/.
   `Archived <https://archive.md/https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/>`__.
   
.. [GS] Gallagher, Sean. “Equifax Hackers Stole Data for 200k Credit Cards from Transaction History.” *Ars Technica*, 14 Sept. 2017, 
   https://arstechnica.com/information-technology/2017/09/equifax-hackers-stole-data-for-200k-credit-cards-from-transaction-history/.
   `Archived <https://archive.md/5Bkbc>`__.

.. [H] Hautala, Laura. “Equifax Ex-CEO: 'Both Human Error and Tech Failures' in Massive Data Breach.” *CNET*, 2 Oct. 2017, 
   https://www.cnet.com/tech/services-and-software/equifax-ceo-data-breach-heres-what-went-wrong/.
   `Archived <https://archive.md/CuNmM>`__.

.. [HA] Hern, Alex. “Equifax Told to Inform Britons Whether They Are at Risk after Data Breach.” *The Guardian*, Guardian News and Media, 8 Sept. 2017, 
   https://www.theguardian.com/technology/2017/sep/08/equifax-told-to-inform-britons-whether-they-are-at-risk-after-data-breach.
   `Archived <https://archive.md/a3PmP>`__.

.. [L] Lomas, Natasha. “Equifax Breach Disclosure Would Have Failed Europe's Tough New Rules.” 
   *TechCrunch*, 8 Sept. 2017, 
   https://techcrunch.com/2017/09/08/equifax-breach-disclosure-would-have-failed-europes-tough-new-rules/.
   `Archived <https://archive.md/ZtPUF>`__.

.. [M] Mathews, Lee. “Equifax Data Breach Impacts 143 Million Americans.” *Forbes*, Forbes Magazine, 7 Sept. 2017,
   https://www.forbes.com/sites/leemathews/2017/09/07/equifax-data-breach-impacts-143-million-americans/?sh=16bb95ef356f.
   `Archived <https://archive.md/fo2um>`__.
   
.. [MM] “Equifax Data Breach Lawsuit.” *Morgan & Morgan*, 
    https://www.forthepeople.com/class-action-lawyers/equifax-data-breach-lawsuit/.
    `Archived <https://archive.md/GRPq3>`__.
   
.. [N] Ng, Alfred. “How the Equifax Hack Happened, and What Still Needs to Be Done.” *CNET*, 7 Sept. 2018, 
   https://www.cnet.com/tech/services-and-software/equifaxs-hack-one-year-later-a-look-back-at-how-it-happened-and-whats-changed/.
   `Archived <https://archive.md/NVeDV>`__.

.. [N2] Ng, Alfred, and Musil, Steven. “Equifax Data Leak May Affect Nearly Half the US Population.” *CNET*, 8 Sept. 2017, 
   https://www.cnet.com/tech/services-and-software/equifax-data-leak-hits-nearly-half-of-the-us-population/.
   `Archived <https://archive.md/dH7ei>`__.

.. [NL] Newman, Lily Hay. “How to Stop the Next Equifax-Style Megabreach-Or At Least Slow It Down.” *Wired*, Conde Nast, 12 Sept. 2017, 
   https://www.wired.com/story/how-to-stop-breaches-equifax/.
   `Archived <https://archive.md/xL7vb>`__.

.. [S] Shepardson, David. “Equifax Failed to Patch Security Vulnerability in March: Former CEO.” *Reuters*, Thomson Reuters, 2 Oct. 2017, 
   https://www.reuters.com/article/us-equifax-breach/equifax-failed-to-patch-security-vulnerability-in-march-former-ceo-idUSKCN1C71VY.
   `Archived <https://archive.md/MJ7zq>`__.

.. [T] Turcsányi, Gergő. “Deep Dive into the Equifax Breach and the Apache Struts Vulnerability.” *Avatao*, 
   https://avatao.com/blog-deep-dive-into-the-equifax-breach-and-the-apache-struts-vulnerability/.
   `Archived <https://archive.md/LPy4G>`__.
   
.. [V] Viswanatha, Aruna, et al. “Four Members of China's Military Indicted Over Massive Equifax Breach.”
   *The Wall Street Journal*, Dow Jones & Company, 11 Feb. 2020,
   https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824.
   `Archived <https://archive.md/JDvB1>`__.
   
.. [VD] Volz, Dustin. “Prosecutors Said PLA's 54th Research Institute-Traditionally Focused 
   on Supporting Electronic Warfare Akin to Cyber Command as Opposed to Cyber Espionage-Was 
   behind the Hack, an Indication the Group's ‘Missions May Be Evolving," @EBKania Said. 
   Https://T.co/dB1bSAsE9h.” Twitter, Twitter, 10 Feb. 2020, 
   https://twitter.com/dnvolz/status/1226983668222132225. 
   `Archived <https://archive.md/Tpwmu>`__.
   
.. [W] Whittaker, Zack. “Equifax Confirms Apache Struts Flaw It Failed to Patch Was to Blame for Data Breach.” 
   *ZDNet*, 13 Sept. 2017, 
   https://www.zdnet.com/article/equifax-confirms-apache-struts-flaw-it-failed-to-patch-was-to-blame-for-data-breach/.
   `Archived <https://archive.md/Qxreg>`__.
   
.. [WE] Weise, Elizabeth, and Nathan Bomey. “Equifax Breach Hit 2.5 Million More Americans than First Believed.” 
   *USA Today*, Gannett Satellite Information Network, 2 Oct. 2017, 
   https://www.usatoday.com/story/tech/2017/10/02/equifax-breach-hit-2-5-million-more-americans-than-first-believed/725100001/.
   `Archived <https://archive.md/TfhLK>`__.
   
.. [WK] “2017 Equifax Data Breach.” *Wikipedia*, Wikimedia Foundation, 25 Oct. 2021, 
   https://en.wikipedia.org/wiki/2017_Equifax_data_breach.
   
.. URLs
.. _29 July 2017: https://www.prnewswire.com/news-releases/equifax-announces-cybersecurity-incident-involving-consumer-information-300515960.html
.. _a months-old issue that Equifax knew about but failed to fix: https://www.cnet.com/news/equifax-ceo-data-breach-heres-what-went-wrong/
.. _Apache Struts: https://struts.apache.org/
.. _Apache Struts software: https://struts.apache.org/
.. _archive: https://web.archive.org/web/20210629150932/https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf
.. _CEO: https://archive.md/1aLaJ
.. _Chinese Military Hackers Charged in Equifax Breach: https://www.fbi.gov/news/stories/chinese-hackers-charged-in-equifax-breach-021020
.. _Chinese Military Officers Hacked Equifax, Justice Department Say: 
   https://www.defenseone.com/technology/2020/02/chinese-military-officers-hacked-equifax-justice-department-says/163013/
.. _CIO and CSO: https://archive.md/qvmvJ
.. _CVE-2017-5638: https://www.cvedetails.com/cve/CVE-2017-5638/
.. _DOJ indictment: https://www.justice.gov/opa/press-release/file/1246891/download
.. _Equifax\: US charges four Chinese military officers over huge hack: 
   https://www.bbc.com/news/world-us-canada-51449778
.. _FBI most wanted: https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute
.. _Four Members of China's Military Indicted for Massive Equifax Breach: 
   https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824
.. _indictment: https://www.justice.gov/opa/press-release/file/1246891/download
.. _Justice Department charges 4 members of Chinese military for massive Equifax hack: 
   https://www.cbsnews.com/news/equifax-hack-chinese-military-members-charged-department-of-justice/
.. _PDF: https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf
.. _press release: https://www.justice.gov/opa/pr/chinese-military-personnel-charged-computer-fraud-economic-espionage-and-wire-fraud-hacking
.. _RT: https://www.rt.com/usa/480536-chinese-military-hackers-equifax/
.. _The US says the Chinese military hacked Equifax. Here’s how.: 
   https://www.technologyreview.com/2020/02/10/349004/the-us-says-the-chinese-military-hacked-equifax-heres-how/
.. _U.S. Charges Chinese Military Officers in 2017 Equifax Hacking: 
   https://archive.md/8EKZs
.. _What is the PLA, and why do feds believe they hacked Equifax?:
   https://www.ajc.com/news/what-the-pla-and-why-feds-believe-they-hacked-equifax/IwFZoHWI4ZEtptRldiD3mJ/
