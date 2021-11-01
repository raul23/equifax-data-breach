========================
2017 Equifax data breach
========================
.. "And how w"And how w"And how w"And how w"And how w"And how w"And how w"And howw

.. raw:: html

   <div align="center">
   <img src="https://www.omegawealthmanagement.com/wp-content/uploads/2020/01/equifax.jpg" style="width:550px;height:250px;"/>
   <p><b><a href="https://www.omegawealthmanagement.com/were-you-affected-by-the-equifax-data-breach-in-2017/">Reference</a></b></p>
   </div>
   
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

  On September 7, 2017, Equifax, one of the largest credit reporting agencies in 
  America, announced that an unauthorized third party gained access to Equifax 
  data on as many as 143 million Americans. [M]_
  
  The number of affected people is roughly half of the US population of 323 
  million. [N2]_
  
`:warning:`

  Equifax learned about the breach on July 29 but didn't reveal it for more than 
  a month. [N2]_

Some important information
==========================
- On March 9, 2017, the company's IT team was informed of a vulnerability 
  affecting the `Apache Struts software`_ it used on its dispute resolution 
  portal, with instructions to patch it in 48 hours. That didn't happen. [H]_
- On May 13, 2017, the attackers hit the jackpot with Equifax's dispute portal, 
  where people could go to argue about claims. [N]_
- The breach was discovered on `29 July 2017`_. [M]_
- On September 7, 2017, Equifax, one of the largest credit reporting agencies 
  in America, announced that an unauthorized third party gained access to 
  Equifax data on as many as 143 million Americans. [M]_
- As a result, the `CEO`_, `CIO and CSO`_ had to go. [T]_
- In both October 2017 [WE]_ and March 2018 [MM]_, Equifax reported that an 
  additional 2.5 and 2.4 million American consumer records were accessed, 
  respectively, bringing the total to 147.9 million. [WK]_

What kinds of data were accessed?
=================================
- The information accessed primarily includes names, Social Security numbers, 
  birth dates, addresses and, in some instances, driver's license numbers. 
  [E]_
  
  The driver's license data of around 10.9 million Americans were compromised. 
  [CM]_

- In addition, credit card numbers for approximately 209,000 U.S. consumers, 
  and certain dispute documents with personal identifying information for 
  approximately 182,000 U.S. consumers, were accessed. [E]_
  
- Equifax also identified unauthorized access to limited personal information 
  for certain UK and Canadian residents. [E]_
  
  Information on an estimated range of under 400,000 up to 44 million British 
  residents. [BBC]_ [HA]_ 
  
  The company said that 8,000 Canadian citizens were impacted. [S]_
  
  An additional 11,670 Canadians were affected as well, later revealed by 
  Equifax. [WK]_ [C]_

How was the data breached?
========================
`:information_source:`

  On 7 September 2018, US lawmakers released a report (`PDF`_ and `archive`_) 
  detailing exactly how the credit-monitoring company was hacked.
  
  The report comes from the Government Accountability Office (GAO), the agency 
  that provides auditing and investigative services for Congess.
  
**Ref.:** `cnet.com <https://www.cnet.com/tech/services-and-software/equifaxs-hack-one-year-later-a-look-back-at-how-it-happened-and-whats-changed/>`__

By exploiting a vulnerability on one of the company's U.S.-based web servers. 
[M]_

It seems that the underlying legacy codebase that handled the [Equifax] web 
application was vulnerable enough for an attacker to exploit. [M]_

1. Hackers used an Apache Struts vulnerability (`CVE-2017-5638`_), `a 
   months-old issue that Equifax knew about but failed to fix`_, and gained 
   access to internal login credentials (for Equifax employees) for three 
   servers. Those credentials allowed them to access 48 credit monitoring 
   databases containing personal information. [N]_ [T]_
2. They searched the databases about 9,000 times for sensitive personal 
   information while hiding the searches through encryption. [B]_
3. They stuffed the personal information in temporary files, compressed them 
   and divided them into smaller-sized files to increase their chances of 
   transmitting the stolen data without being noticed. [B]_ [N]_
4. They used 34 servers in 20 countries during the breach and employed various 
   other techniques, such as remote-desktop access and encrypted log-ins, to 
   mask the origin of the hack. [B]_
5. They deleted the compressed files after transferring the data into external 
   storage, then configured settings to wipe out information tracking their 
   activity. [B]_
6. The thieves spent 76 days within Equifax's network before they were 
   detected. [N]_

`:information_source:`

  While the failure to update Struts was a key failure, analysis of the breach 
  found further faults in Equifax' system that made it easy for the breach to 
  occur, including [WK]_:
  
  - the insecure network design which lacked sufficient segmentation [NL]_
  - potentially inadequate encryption of personally identifiable information 
    (PII) [GS]_, and
  - ineffective breach detection mechanisms. [L]_

.. raw:: html

   <div align="center">
   <img src="https://camo.githubusercontent.com/4dbe1733c0ea00a63c6096fef006392d8544b2ef9e8947f3aafca507ba7837a1/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f313430302f302a46334476476b37755234583538613566" style="width:700px;height:500px;"/>
   <p><b>A chart from the <a href="https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf">GAO report</a>
      describing how Equifax was breached.</b></p>
   </div>
   
List of malware files and web shells used by the hackers
========================================================
`:information_source:`

  This list is compiled from the United States Department of Justice 
  (DOJ) `indictment`_ that was unsealed on February 10, 2020.
  
TODO
   
The US says members of the Chinese military hacked Equifax
==========================================================
`:warning:`

  The United States Department of Justice (DOJ) is very careful not to imply 
  that the Chinese army is directly responsible for the data breach.
  Thus, the `DOJ indictment`_ and their `press release`_ target specifically 
  members of the Chinese People’s Liberation Army (PLA); more precisely they 
  are part of PLA’s 54th Research Institute, a component of the Chinese 
  military.
  
  The majority of mainstream news sites are also careful in their titles so as 
  to be specific in who are being accused by the DOJ:

  - `Chinese Military Hackers Charged in Equifax Breach`_ (FBI News)
  - `Chinese Military Officers Hacked Equifax, Justice Department Say`_ (
    Defense One)
  - `Equifax: US charges four Chinese military officers over huge hack`_ (BBC 
    News)
  - `Four Members of China's Military Indicted for Massive Equifax Breach`_ (
    The Wall Street Journal)
  - `Justice Department charges 4 members of Chinese military for massive 
    Equifax hack`_ (CBS NEWS)
  - `U.S. Charges Chinese Military Officers in 2017 Equifax Hacking`_ (The New 
    York Times)
  
  Though you still have some news articles with titles implying that it is the 
  whole Chinese army that is being targeted by the DOJ:

  - `US says China's military was behind 2017 Equifax hack that left personal 
    information of 145 million Americans exposed`_ (Business Insider)
  - `What is the PLA, and why do feds believe they hacked Equifax?`_ (The 
    Atlanta Journal-Constitution)
  - `The US says the Chinese military hacked Equifax. Here’s how.`_ (MIT 
    Technology Review)
  - `Report: Chinese Army Stole Over 13 Million British Citizens’ 
    Personal Data`_ (Breitbart)

|

`:warning:`

  Also, it is very important to keep in mind that what is written in the DOJ 
  `indictment`_ is based on allegations and people (especially media pundits) 
  should not repeat what is in the document as gospel.
  
That's why the DOJ `press release`_ says the following in the bottom of the
page (emphasis mine):
  
  The details contained in the charging document are **ALLEGATIONS**.  
  The defendants are presumed innocent until proven guilty beyond a 
  reasonable doubt in a court of law.
    
And here is the definiton for the word "allegation" (emphasis mine):
  
  a statement, made **WITHOUT GIVING PROOF**, that someone has done 
  something wrong or illegal [CA]_

The US indictment
-----------------
On February 10, 2020, the DOJ indicted four members of 
China's military on nine charges related to the hack. [DOJ]_

From the DOJ press release about the `indictment`_ 
(`archive <https://web.archive.org/web/20210725031951/https://www.justice.gov/opa/press-release/file/1246891/download>`__) 
of the four Chinese military members [DOJ]_:

  The nine-count indictment alleges that Wu Zhiyong (吴志勇), Wang Qian (王乾), 
  Xu Ke (许可) and Liu Lei (刘磊) were members of the PLA’s 54th Research 
  Institute, a component of the Chinese military.  They allegedly conspired 
  with each other to hack into Equifax’s computer networks, maintain 
  unauthorized access to those computers, and steal sensitive, personally 
  identifiable information of approximately 145 million American victims. 

|

`:warning:`

In the DOJ `indictment`_, it is claimed that the four alleged PLA hackers 
also conspired with other people that are known and unknown to the DOJ 
(emphasis mine):
  
- From the "Count 1: Computer Fraud Conspiracy)" section of the DOJ 
  `indictment`_:

     ... the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, did 
     knowingly and willfully combine, conspire, confederate, agree, and have a 
     tacit understanding with each other and **OTHER PERSONS KNOWN AND 
     UNKNOWN** to the Grand Jury ...
     
     [DOJ2]_ (*paragraph 6, page 4*)

- From the OVERT ACTS subsection of "Count 1" of the DOJ `indictment`_:

     ... the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, and 
     **OTHERS** committed various overt acts in the Northern District of 
     Georgia and elsewhere ...
     
     [DOJ2]_ (*paragraph 14, page 7*)

- From the "Count 2: Computer Fraud and Abuse (Intentional Damage)" section of 
  the DOJ `indictment`_:

     ... the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, aided and 
     abetted by each other and **OTHERS KNOWN AND UNKNOWN** to the Grand Jury
     ...
     
     [DOJ2]_ (*paragraph 16, pages 11-12*)
     
- From the "Count 3: Computer Fraud and Abuse: Unauthorized Access" section of 
  the DOJ `indictment`_:
    
     the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, aided and 
     abetted by each other and **OTHERS KNOWN AND UNKNOWN** to the Grand 
     Jury

     [DOJ2]_ (*paragraph 18, page 12*)
     
- From the "Count 4: Conspiracy to Commit Economic Espionage" section of 
  the DOJ `indictment`_:
    
     the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, knowingly 
     and willfully combined, conspired, confederated, agreed, and had a 
     tacit understanding, with each other and **OTHERS KNOWN AND UNKNOWN** 
     to the Grand Jury

     [DOJ2]_ (*paragraph 20, page 13*)

- From the OVERT ACTS subsection of "Count 4" of the DOJ `indictment`_:

     ... the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, and 
     **OTHERS** committed various overt acts in the Northern District of 
     Georgia and elsewhere ...
     
     [DOJ2]_ (*paragraph 21, page 14*)
     
- From the "Count 5: Economic Espionage" section of the DOJ 
  `indictment`_:
     
     ... the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, aided 
     and abetted by each other and **OTHERS KNOWN AND UNKNOWN** to the Grand 
     Jury ...
 
     [DOJ2]_ (*paragraph 23, page 14*)

- From the "Count 6: Conspiracy to Commit Wire Fraud" section of the DOJ 
  `indictment`_:
     
     ... the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, 
     knowingly and willfully combined, conspired, confederated, agreed, and 
     had tacit understanding, with each other and **OTHERS KNOWN AND 
     UNKNOWN** to the Grand Jury ...
 
     [DOJ2]_ (*paragraph 25, page 15*)

- From the MANNER AND MEANS OF THE CONSPIRACY subsection of "Count 6" 
  of the DOJ `indictment`_:

     1. It was part of the conspiracy that the defendants, WU ZHIYONG, 
        WANG QIAN, XU KE, and LIU LEI, and **OTHERS KNOWN AND UNKNOWN** ...
     
        [DOJ2]_ (*paragraph 26, page 16*)
     
     2. After infiltrating Equifax's network, WU ZHIYONG, WANG QIAN, XU 
        KE, and LIU LEI, and their **CO-CONSPIRATORS** ...
     
        [DOJ2]_ (*paragraph 27, page 16*)
     
     3. WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, and their 
        **CO-CONSPIRATORS** ...
     
        [DOJ2]_ (*paragraph 28, page 16*)
       
     4. After gaining access to these additional databases with stolen 
        credentials, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, and their 
        **CO-CONSPIRATORS** ...
     
        [DOJ2]_ (*paragraph 29, page 16*)

- From the "Counts 7 through 9: Wire Fraud" section of the DOJ 
  `indictment`_:
     
     ... the defendants, WU ZHIYONG, WANG QIAN, XU KE, and LIU LEI, 
     aided and abetted by each other and **OTHERS KNOWN AND UNKNOWN** 
     to the Grand Jury,
 
     [DOJ2]_ (*paragraph 31, page 17*)
     
DOJ evidence that China's military personnel are behind the Equifax data breach
-------------------------------------------------------------------------------
`:information_source:`

  These are evidence that I was able to gather from the DOJ `indictment`_. 
  
  **TODO:** gather evidence from other governmental sources if they are found
  
1. Multiple China-based IP addresses were allegedly accessed during the 
   intrusion of Equifax's networks by the conspirators:

   - The majority of the 9000 SQL queries [to the credit monitoring databases] 
     were issued by conspirators using two **China-based IP addresses** that 
     connected directly to Equifax' s network. [DOJ2]_ (*paragraph 9, page 6*)

     **NOTE:** the indictment doesn't name these two **China-based IP 
     addresses** like in other places of the document (e.g. China Server #1)
   - **China Server #1:** On or about June 16, 2017, a conspirator using a 
     China-based IP address ("China Server #1"), which was repeatedly accessed 
     during the intrusion by WANG QIAN, logged into a Taiwanese IP address (
     "the Taiwan Server") via Remote Desktop Protocol software and copied the 
     malicious file "jndi. txt." [DOJ2]_ (*paragraph 14.e, page 8*)
   - **China Server #2:** On or about July 7, 2017, another China-based IP 
     address ("China Server #2"), which was also repeatedly accessed during 
     the intrusion by WANG QIAN, exploited the Apache Struts vulnerability on 
     Equifax' s online dispute portal. [DOJ2]_ (*paragraph 14.j, page 9*)
   - **China Server #3:** On or about July 9, 2017, XUKE used a different 
     China-based IP address ("China Server #3") to conduct reconnaissance on 
     Equifax' s online dispute portal. [DOJ2]_ (*paragraph 14.k, page 10*)
   - **China Server #4:** On or about July 10, 2017, a conspirator using 
     another China-based IP address ("China Server #4") logged into the Taiwan 
     Server and copied the malicious file "abc.txt" to the Taiwan Server. 
     [DOJ2]_ (*Paragraph 14.l, page 10*)
   - **China Server #5:** On or about July 10, 2017, a conspirator using 
     another China-based IP address ("China Server #5'') then utilized the 
     malicious web shell ''css.jsp," which was previously installed on 
     Equifax's network, to issue a command to download the "abc. txt" file 
     from the Taiwan Server. [DOJ2]_ (*paragraph 14.l, page 10*)
   - **China Server #6:** On or about July 10, 2017, a conspirator who was 
     logged into another China-based IP address ("China Server #6") utilized 
     the malicious web shell ''boxover.jsp" to query an Equifax database table 
     and store the results in output files. [DOJ2]_ (*paragraph 14.n, page 10*)
 
   `:information_source:`
   
     Reading the DOJ `indictment`_, you have the impression that the US 
     authorities were somehow able to exactly pinpoint who among the four 
     alleged members of the PLA logged to Equifax's networks at a particular 
     time of the day.
     
     However for some other days of the attack, the US investigators lose 
     their special skill to exactly identify who is logging into Equifax's 
     networks and instead used the word "conspirator".
   
   `:information_source:`

     The conspirators also allegedly accessed IP addresses from locations 
     outside of China:
   
     - Switzerland ("the Swiss Server"), [DOJ2]_ (*paragraph 14.f, page 9*)
     
       According to the DOJ `indictment`_, the Swiss Server was accessed 5 
       times by the conspirators.
       
     - Taiwan ("the Taiwan Server"), [DOJ2]_ (*paragraph 14.e, page 8*)
     
       According to the DOJ `indictment`_, the Taiwan Server was accessed 3
       times by the conspirators.

     - Netherlands [DOJ2]_ (*paragraph 14.m, page 10*)
     
       According to the DOJ `indictment`_, the Dutch server was accessed one
       time by the conspirators.
     
     - Singapore ("the Singapore Server") [DOJ2]_ (*paragraph 14.o, page 11*)
     
       According to the DOJ `indictment`_, the Singapore Server was accessed 2
       times by the conspirators.
       
2. By stealing Equifax's **trade secrets** (including the personally 
   identifiable data and the proprietary database schema), it is claimed by 
   the DOJ that the alleged Chinese hackers are working with the Chinese
   government and the PLA because these are the kinds of data that these 
   entities are interested in (emphasis mine):
   
     ... with said **TRADE SECRETS** [...], intending and knowing that the 
     offense would **BENEFIT A FOREIGN GOVERNMENT**, instrumentality, and 
     agent, namely **CHINA AND THE PEOPLE'S LIBERATION ARMY**, in violation 
     of Title 18, United States Code, Sections 1831(a)(1), (a)(2), and (a)(3).
     
     [DOJ2]_ (*paragraph 20, pages 13-14*)
     
     |
     
     ... the defendants [...] intending and knowing that the offense would 
     **BENEFIT A FOREIGN GOVERNMENT**, instrumentality, and agent, namely 
     **CHINA AND THE PEOPLE'S LIBERATION ARMY**, did knowingly and without 
     authorization copy, duplicate, download, upload, replicate, transmit, 
     deliver, send, mail, communicate, and convey a **TRADE SECRET** ...
     
     [DOJ2]_ (*paragraph 23, pages 14-15*)

DOJ evidence: weak
------------------
The evidence gathered from the DOJ `indictment`_ is very weak to support the 
claim that four alleged members of the PLA were the perpetrators of the Equifax 
data breach.

- No much information is given about the four suspected PLA members: Wu Zhiyong 
  (吴志勇), Wang Qian (王乾), Xu Ke (许可) and Liu Lei (刘磊).

  The DOJ `indictment`_ and mainstream news articles only provide their names, 
  pictures, and Beijing, China as their location of residence. However in the
  indictment, Beijing is referred in the past (emphasis mine):
  
    Defendants [...] **WERE** residents of Beijing, China 
    
    [DOJ2]_ (*parapraph 5.d, pages 3-4*)
    
  Thus, the whereabouts of the suspects are uncertain.
  
  Also, from the DOJ `indictment`_ and `press release`_, it seems that they 
  refer to the four suspects as being former members of PLA's 54th Research 
  Institute (emphasis mine):
  
    Defendants [...] **WERE** members of the 54th Research Institute, which 
    **WAS** a component of the PLA. 
    
    [DOJ2]_ (*parapraph 5.d, pages 3-4*)
  
  |
  
    ... Wu Zhiyong (吴志勇), Wang Qian (王乾), Xu Ke (许可) and Liu Lei (刘磊) 
    **WERE** members of the PLA’s 54th Research Institute, a component of 
    the Chinese military. [DOJ]_
    
  From the previous two quotes, is the 54th Research Institute still a 
  component of the PLA? 
  
  Their `FBI most wanted`_ poster and the `FBI news article`_ only give their 
  names and pictures but don't mention Beijing which should have been included 
  since it is presumably an important information for people to help the FBI 
  identify the four suspects. At least, the FBI should have said that the 
  four alleged PLA hackers are probably still living in Beijing, China.
  
  More information (basic and detailed) is about the four alleged PLA hackers 
  such as: 
  
  - General questions about their life: How old are they? Where did they grew 
    up? Where did they study? Where did they work, apart from the PLA?
    Did they leave China at one point in their life?
  - Are Wang Qian and Liu Lei (the only ones not wearing military uniforms in 
    the pictures) civilians working for PLA's 54th Research Institute or 
    active-duty members of the PLA? 
  - What are their military ranks in the PLA? 
  - Were they receiving orders from higher up or were they acting on their 
    own? 
  - Where are those pictures provided in the `indictment`_ of three of 
    the four PLA members coming from? 
  
  All those questions are important for the FBI, DOJ, CIA, and any other relevant 
  three letter agencies to answer to the public because this is the kind of 
  information that will be useful for anyone around the world to be able to 
  recognize any of the alleged PLA hackers. Only in China, there are 
  approximately `1.412 billion people`_ (as of November 2020) and the more 
  personal information you give, higher will be the chance for someone to produce
  helpful tips.
  
  But right now, the personal info the DOJ et al. have provided is very weak and
  doesn't help much the public to identify the four alleged hackers.
  
  There is still the possibility that any of the alleged hackers might leave China 
  in the near future and go to a place that they think there is no extradition 
  treaty with the US, not knowing that the US can still apprehend them (they
  are a superpower after all). Just take the example of the Russian hacker 
  `Roman Seleznev`_ that thought that he was safe in the Maldives because they 
  don't have an extradition treaty with the U.S. `He thought wrong`_.
  
  .. raw:: html

     <div align="center">
     <img src="https://www.cnet.com/a/img/uf_P-IUAQf-_-47zXmpuSWcyqs8=/940x0/2020/02/10/489560f1-9731-4957-af0d-9b0a947da334/screen-shot-2020-02-10-at-10-18-15-am.png" style="width:700px;height:400px;"/>
     <p><b>In the news articles and the DOJ <a href="https://www.justice.gov/opa/press-release/file/1246891/download">indictment</a>, they don't provide a picture for the alleged PLA member Liu Lei.
        However in the <a href="https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute">FBI poster</a>, 
        you get all four pictures (though <a href="https://archive.md/3qA8b">at first</a> the FBI also only shown three pics). Very odd that the DOJ et al. worked for 2 years investigating the Equifax data breach
        and could not get a picture for Liu Lei to include in their indictment.</b></p>
     </div>
     
  |
  
  .. raw:: html

     <div align="center">
     <img src="https://www.fbi.gov/@@dvpdffiles/8/c/8c0b4ce2b3c9448b95b13f19a89fc658/normal/dump_1.gif"/>
     <p><b>PLA members wanted by the
       <a href="https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute">FBI</a>.</b></p>
     </div>
     
  And to finish this mega huge bullet point on a lighter note, `SecureWorld`_ believes 
  that the pictures provided by the DOJ and FBI support the idea that the four 
  supposedly identified hackers are all working in the Chinese military. Also, 
  they state that the cyberattack on Equifax's networks was pulled off from Shanghai, 
  China.
  
  .. raw:: html

     <div align="center">
       <img src="https://memegenerator.net/img/images/71799850.jpg" style="width:300px;height:200px;"/>
     </div>

- There is no explanation in the `indictment`_ how the US authorities came to 
  the conclusion that the four alleged PLA members were directly related to the 
  network intrusions of Equifax computers.

- Some of the evidence is based on multiple IP addresses allegedly originating 
  from China.

  It seems very sloppy for the four alleged members of the PLA to reportedly 
  log multiple times into Equifax's systems directly from China-based IP 
  addresses. These conspirators are not your average Joe that doesn't know much 
  about network forensics but are supposedly part of PLA's 54th Research 
  Institute which has traditionally focused on supporting electronic warfare 
  akin to Cyber Command as opposed to cyber espionage [VD]_. 
  
  Therefore, these four alleged PLA members should know very well how to hide 
  their tracks and use only IP addresses from outside China. 
  
  The four suspected PLA hackers and their alleged co-conspirators were able 
  to navigate throughout Equifax's networks as mere ghosts. To achieve their 
  cloak of anonymity, they supposedly: 
  
    - routed traffic through approximately 34 servers located in nearly 20 
      countries to obfuscate their true location, 
    - used encrypted communication channels within Equifax’s network to blend 
      in with normal network activity, and 
    - deleted compressed files and wiped log files on a daily basis in an 
      effort to eliminate records of their activity. [DOJ]_
      
  But according to the DOJ `indictment`_, the four alleged `elite`_ 
  hackers and their supposedly co-conspirators **DIRECTLY** accessed 
  China-based IP addresses multiple times during their 2-month attack. This 
  is a very basic and surprising mistake to commit when "hiding their tracks" is 
  supposed to be the most important thing to accomplish because the network 
  intrusions rest on constantly keeping the anonymity of the attackers. 
  Accessing servers only from outside of China was not rigidly followed by 
  the alleged group of hackers unless they really wanted to be identified 
  and didn't care about repercussions (emphasis mine):
  
    1. The majority of the 9000 SQL queries [to the credit monitoring databases] 
       were issued by conspirators using two **CHINA-BASED** IP addresses that 
       connected **DIRECTLY** to Equifax' s network.
    
       [DOJ2]_ (paragraph 9, page 6)
      
    2. ... another **CHINA-BASED** IP address ("China Server #2"), which was 
       also repeatedly accessed during the intrusion by WANG QIAN, exploited 
       the Apache Struts vulnerability on Equifax's online dispute portal. 
      
       [DOJ2]_ (paragraph 14.j, pages 9-10)
      
    3. ... XU KE used a different **CHINA-BASED** IP address ("China Server #3") 
       to conduct reconnaissance on Equifax's online dispute portal. 
      
       [DOJ2]_ (paragraph 14.k, page 10)
      
    4. A conspirator using another **CHINA-BASED** IP address ("China Server #5") 
       then utilized the malicious web shell "css.jsp," whichwas previously 
       installed on Equifax's network ...
      
       [DOJ2]_ (paragraph 14.l, page 10)
      
    5. ... a conspirator using **CHINA** Server #5 uploaded a substantively 
       identical web shell, "ss.jsp," to the Equifax network. 
    
       [DOJ2]_ (paragraph 14.l, page 10)
       
    6. ... a conspirator who was logged into another **CHINA-BASED** IP address 
       ("China Server #6") utilized the malicious web shell "boxover.jsp" to 
       query an Equifax database table ...
       
       [DOJ2]_ (paragraph 14.n, page 10)
       
    7. ... WANG QIAN, using **CHINA** Server #2, remotely accessed the 
       malicious web shell "six.jsp" on an Equifax server ...
       
       [DOJ2]_ (paragraph 14.o, page 11)
    
  The suspected hackers supposedly had the backing of the `second most 
  important army in the world in terms of budget`_ (for 2020) but they were 
  not able to think of various ways of definitely hiding their tracks that 
  didn't require frequently logging from the same country. It would had been 
  extremely careless of China to not make sure to be as anonymous as possible 
  because they certainly knew that if they didn't, they risked further 
  deteriorating their tense diplomatic relations with the currently only 
  military superpower that is the USA which had `accused China`_ of multiple 
  cyberattacks against the US and allies (e.g. the `2015 massive breach at the 
  U.S. Office of Personnel Management`_).
  
- Since it is extremely unlikely for the DOJ to arrest the four alleged PLA 
  members, the quality of the evidence in the `indictment`_ can be very poor. 
  The case will likely not go in front of a judge and jury where the evidence 
  presented by the prosecutors would have been scrutinized.
  
  Thus, the DOJ is not incentivized to gather solid evidence that could link 
  the four alleged PLA members to the Equifax data breach:
  
    Officials acknowledged they were unlikely to face prosecution in a U.S. 
    courtroom. [V]_ 

Reading the many mainstream news articles (even outside the USA like UK and 
Canada), you get the feeling that everyone just went along with the narrative of 
the DOJ that four PLA members are unequivocally responsible for the Equifax 
data breach.

However, `RT.com`_ is among the only news sites that questioned the link 
between the four alleged PLA members and the data breach as promulgated by the 
DOJ:

  It remains unclear how the DOJ concluded that four members of the Chinese 
  military were responsible, whether they were supposedly acting on their own or 
  on state orders, or how it intends to bring them to a US court. [RT]_

Since it is from RT, people (especially in the US) will have a tendency to 
discard whatever they have to say because they are `"the Kremlin's 
foreign-language propaganda network"`_.

Also `tom's guide`_ asked important questions about the DOJ `indictment`_ 
claiming that the four suspected Chinese hackers were allegedly military 
members of the PLA:

  It is not clear whether the four individuals are civilians working for the 
  PLA or active-duty members of the Chinese military. No military ranks were 
  given for any of the defendants in the indictment, but the four were said to 
  be members of the PLA's 54th Research Institute. (Update: A `wanted poster 
  put up online by the FBI`_ shows photos allegedly of Wu and Xu wearing 
  military uniforms.) [WP]_

Non-DOJ evidence that China's military personnel are behind the Equifax data breach
-----------------------------------------------------------------------------------
`:information_source:`

  These are evidence that I was able to gather from non governmental sources such as 
  from mainstream newspapers. However, as you may see, the information provided by
  journalisys will probably come from anonymous sources and hence their statements
  may prove difficult (or almost impossible) to corroborate.
  
.. TODO: add more non governmental sources
  
TODO
  
Non-DOJ evidence: weak
----------------------
TODO

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
    to arrest them if they travel one day. [FA]_

Technical questions 
===================
For technical questions relating to the 2017 Equifax data breach such as "How 
did the hackers hide their tracks?" or "How web shells were used by the 
hackers?", check the `Technical questions`_ page.

Glossary
========
.. TODO: add definitions

- Chinese People’s Liberation Army (PLA)
- The Government Accountability Office (GAO)
- Personally identifiable information (PII)
- The United States Department of Justice (DOJ)

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
  
- Cimpanu, Catalin. `“US Government Releases Post-Mortem Report on Equifax Hack.” 
  <https://www.zdnet.com/article/us-government-releases-post-mortem-report-on-equifax-hack/>`__ 
  *ZDNet*, 7 Sept. 2018.
  `Archived <https://archive.md/vhgUj>`__.

- O'Flaherty, Kate. `“Equifax Lawsuit: 'Admin' As Password At Time Of 2017 Breach.” 
  <https://www.forbes.com/sites/kateoflahertyuk/2019/10/20/equifax-lawsuit-reveals-terrible-security-practices-at-time-of-2017-breach/>`__ 
  *Forbes*, Forbes Magazine, 20 Oct. 2019. `Archived <https://archive.md/DbHFJ>`__.

- “Criminal Indictment: UNITED STATES OF AMERICA *v.* WU ZHIYONG, WANG 
  QIAN, XUKE, LIU LEI” *The United States Department of Justice*, 28 Jan. 
  2020, https://www.justice.gov/opa/press-release/file/1246891/download (PDF).
  `Archived <https://web.archive.org/web/20210702191105/https://www.justice.gov/opa/press-release/file/1246891/download>`__.

- `“Press Release: Chinese Military Personnel Charged with Computer Fraud, 
  Economic Espionage and Wire Fraud for Hacking into Credit Reporting Agency 
  Equifax.” 
  <https://www.justice.gov/opa/pr/chinese-military-personnel-charged-computer-fraud-economic-espionage-and-wire-fraud-hacking>`__
  *The United States Department of Justice*, 10 Feb. 2020.
  `Archived <https://archive.md/JtDCY>`__. 

- `“Chinese Hackers Charged in Equifax Breach.” 
  <https://www.fbi.gov/news/stories/chinese-hackers-charged-in-equifax-breach-021020>`__ 
  *FBI*, 10 Feb. 2020.
  `Archived <https://archive.md/https://www.fbi.gov/news/stories/chinese-hackers-charged-in-equifax-breach-021020>`__.

- `“CHINESE PLA MEMBERS, 54th RESEARCH INSTITUTE.” 
  <https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute>`__ 
  *FBI*, 10 Feb. 2020. `Archived#1 <https://archive.md/3qA8b>`__ (10 Feb. 2020) and 
  `Archived#2 <https://web.archive.org/web/20211020075542/https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute>`__ (20 Oct. 2021).

- Fbi. “Wu Zhiyong, Wang Qian, Xu Ke, and Liu Lei Face Charges of Computer 
  Fraud, Economic Espionage, and Wire Fraud for Their Role in One of the Largest 
  Thefts of Personally Identifiable Information by State-Sponsored Hackers Ever 
  Recorded. Https://T.co/KcZ8lOfpbd Pic.twitter.com/65vDyh4HTx.” 
  *Twitter*, 10 Feb. 2020, https://twitter.com/FBI/status/1226896376971300865.
  `Archived <https://archive.md/MSgsh>`__.
  
- Associated Press. `“US Charges 4 Chinese Military Members in Equifax Breach.” 
  <https://www.dailymail.co.uk/news/article-7987465/US-charges-4-Chinese-military-hackers-Equifax-breach.html>`__ 
  *Daily Mail Online*, Associated Newspapers, 10 Feb. 2020.
  `Archived <https://archive.md/pzBkl>`__.

- Baksh, Mariam. `“Chinese Military Officers Hacked Equifax, Justice Department Says.” 
  <https://www.defenseone.com/technology/2020/02/chinese-military-officers-hacked-equifax-justice-department-says/163013/>`__ 
  *Defense One*, Nextgov, 10 Feb. 2020.
  `Archived <https://archive.md/esWq6>`__.

- Barrett, Brian. `“How 4 Chinese Hackers Allegedly Took Down Equifax.” 
  <https://www.wired.com/story/equifax-hack-china/>`__ 
  *Wired*, Conde Nast, 10 Feb. 2020. `Archived <https://archive.md/wj8kZ>`__.

- Benner, Katie. `“U.S. Charges Chinese Military Officers in 2017 Equifax Hacking.” 
  <https://www.nytimes.com/2020/02/10/us/politics/equifax-hack-china.html>`__ 
  *The New York Times*, 10 Feb. 2020.
  `Archived <https://archive.md/https://www.nytimes.com/2020/02/10/us/politics/equifax-hack-china.html>`__.

- Bomey, Nathan. `“How Chinese Military Hackers Allegedly Pulled off the Equifax Data Breach, Stealing Data from 145 Million Americans.” 
  <https://www.usatoday.com/story/tech/2020/02/10/2017-equifax-data-breach-chinese-military-hack/4712788002/>`__
  *USA Today*, Gannett Satellite Information Network, 10 Feb. 2020.
  `Archived <https://archive.md/tMyN3>`__.
  
- Deschamps, Tara. `“Chinese Military Members Face Charges in Equifax Breach Impacting Canadians.” 
  <https://www.ctvnews.ca/business/chinese-military-members-face-charges-in-equifax-breach-impacting-canadians-1.4805070>`__ 
  *CTVNews*, 10 Feb. 2020.
  `Archived <https://archive.md/Lzt3U>`__.
  
- Holmes, Aaron. `“US Says China's Military Was behind 2017 Equifax Hack That Left 
  Personal Information of 145 Million Americans Exposed.” 
  <https://www.businessinsider.com/doj-china-pla-military-hackers-indicted-equifax-2017-breach-2020-2>`_ 
  *Business Insider*, 10 Feb. 2020.
  `Archived <https://archive.md/LFpEv>`__.
  
- Linder, Courtney. `“How Chinese Military Officers Allegedly Hacked Equifax.” 
  <https://www.popularmechanics.com/technology/security/a30854291/equifax-data-breach-chinese-military/>`__
  *Popular Mechanics*, 10 Feb. 2020. `Archived <https://archive.md/liXPo>`__.
  
- Martin, Alexander. `“US Charges Chinese Military Hackers with Equifax Breach.” 
  <https://news.sky.com/story/us-charges-chinese-military-hackers-with-equifax-breach-11930927>`__ 
  *Sky News*, 10 Feb. 2020. `Archived <https://archive.md/jgrRQ>`__.
  
- Murphy, Margi. `“Chinese Military Hackers Charged with Equifax Cyber Attack 
  That Hit 15m Britons.” 
  <https://www.telegraph.co.uk/technology/2020/02/10/chinese-military-hackers-charged-equifax-cyber-attack-hit-15m/>`__ 
  *The Telegraph*, Telegraph Media Group, 10 Feb. 2020.
  `Archived <https://archive.md/ICs75>`__.
  
- News Wires. `“US Charges Four Chinese Military Officers in 2017 Equifax Hack.” 
  <https://www.france24.com/en/20200210-us-charges-four-chinese-military-officers-in-2017-equifax-hack>`__ 
  *France 24*, 10 Feb. 2020.
  `Archived <https://archive.md/9Ncmj>`__.
  
- O'Neill, Patrick Howell. `“The US Says the Chinese Military Hacked Equifax. 
  Here's How.” 
  <https://www.technologyreview.com/2020/02/10/349004/the-us-says-the-chinese-military-hacked-equifax-heres-how/>`__ 
  *MIT Technology Review*, 10 Feb. 2020. `Archived <https://archive.md/VINHI>`__.
  
- Riotta, Chris. `“US Charges Chinese Military Hackers over Cyber-Attack of Equifax.” 
  <https://www.independent.co.uk/news/world/americas/equifax-hack-china-cyber-attack-credit-score-latest-a9327611.html>`__
  *The Independent*, Independent Digital News and Media, 10 Feb. 2020.
  `Archived <https://archive.md/8Yjyx>`__.

- RT. `“Blaming Beijing: US Charges 4 Chinese Military Personnel over Massive Equifax Hack.” 
  <https://www.rt.com/usa/480536-chinese-military-hackers-equifax/>`__ 
  *RT International*, 10 Feb. 2020. `Archived <https://archive.md/dEYcR>`__.

- Sussman, Bruce. `“Equifax Hackers Charged: How the Chinese Did It.” 
  <https://www.secureworld.io/industry-news/equifax-hacker-indictment-10-fast-facts>`_ 
  *SecureWorld*, 10 Feb. 2020.
  `Archived <https://archive.md/a1TQE>`__.

- The Associated Press. 
  `“U.S. Charges 4 Chinese Military Hackers in Equifax Breach Probe | CBC News.” 
  <https://www.cbc.ca/news/business/us-justice-charges-china-equifax-1.5458110>`__ 
  *CBCnews*, CBC/Radio Canada, 10 Feb. 2020.
  `Archived <https://archive.md/aSjVO>`__.

- Tuckers, Eric, and Balsamo, Michael. 
  `“4 Chinese Military Members Charged by U.S. in Equifax Breach - National.” 
  <https://globalnews.ca/news/6530660/equifax-breach-chinese-military-charge/>`__ 
  *Global News*, 10 Feb. 2020. `Archived <https://archive.md/Cj0Li>`__.

- Viswanatha, Aruna, et al. `“Four Members of China's Military Indicted Over 
  Massive Equifax Breach.” 
  <https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824>`__ 
  *The Wall Street Journal*, Dow Jones & Company, 10 Feb. 2020.
  `Archived 
  <https://web.archive.org/web/20211009220413/https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824>`__.
  
- Wagenseil, Paul. `“Equifax Data Breach Was China's Doing, According to the US Government.” 
  <https://www.tomsguide.com/uk/news/equifax-hack-china-charges>`__ 
  *Tom's Guide*, 10 Feb. 2020. `Archived <https://archive.md/Pq3ut>`__.

- `“Data from Equifax Credit Hack Could ‘End up on the Black Market," Expert Warns.” 
  <https://www.cbsnews.com/news/china-denies-responsibility-in-equifax-breach-after-doj-charges-four-military-members/>`__ 
  *CBS News*, CBS Interactive, 11 Feb. 2020. `Archived <https://archive.md/7F470>`__.
  
- `“Equifax: US Charges Four Chinese Military Officers over Huge Hack.” 
  <https://www.bbc.com/news/world-us-canada-51449778>`__ 
  *BBC News*, BBC, 11 Feb. 2020. `Archived <https://archive.md/6kwbg>`__.

- Hymes, Clare, and Becket, Stepan. `“Justice Department Charges 4 Members of Chinese Military for Massive Equifax Hack.” 
  <https://www.cbsnews.com/news/equifax-hack-chinese-military-members-charged-department-of-justice/>`__
  *CBS News*, CBS Interactive, 11 Feb. 2020. `Archived <https://archive.md/NZZIs>`__.

- Jowitt, Tom. `“US Charges Four Chinese Military Over Equifax Hack: Silicon UK Tech News.” 
  <https://www.silicon.co.uk/security/cyberwar/us-charges-chinese-military-equifax-hack-331572>`__ 
  *Silicon UK*, 11 Feb. 2020. `Archived <https://archive.md/x8FCO>`__.
  
- Ng, Alfred. `“China Denies Equifax Hack after Justice Department Charged Four Military Hackers.” 
  <https://www.cnet.com/news/china-denies-equifax-hack-after-justice-department-charged-four-military-hackers/>`_ 
  *CNET*, 11 Feb. 2020. `Archived <https://archive.md/VVTSL>`__.
  
- Mozur, Paul. `“With Harsh Words, China's Military Denies It Hacked Equifax.” 
  <https://www.nytimes.com/2020/02/13/business/china-equifax-deny.html>`_ 
  *The New York Times*, 13 Feb. 2020. `Archived <https://archive.md/WeO4Y>`__.
  
- Gadher, Dipesh. `“Chinese Army's Elite Hackers Steal Equifax Data on 13m Britons.” 
  <https://www.thetimes.co.uk/article/chinese-armys-elite-hackers-steal-equifax-data-on-13m-britons-ld32rqjqq>`__ 
  *The Sunday Times*, 16 Feb. 2020. `Archived <https://archive.md/4kCSs>`__.
  
- Zindulka, Kurt. `“Report: China Stole the Personal Data of Over 13 Million UK Citizens.” 
  <https://www.breitbart.com/europe/2020/02/17/equifax-hack-china-stole-13-million-peoples-data-in-the-uk/>`__ 
  *Breitbart*, 17 Feb. 2020. `Archived <https://archive.md/d9bJ7>`__.

- Fifield, Anna. `“China Rebuffs U.S. Charges of Cyberespionage over Equifax 
  Hack.” 
  <https://www.washingtonpost.com/world/asia_pacific/china-rebuffs-american-charges-of-cyber-espionage-over-equifax-hack/2020/02/11/b95fd932-4ca2-11ea-967b-e074d302c7d4_story.html>`__ 
  *The Washington Post*, WP Company, 20 Feb. 2020. `Archived <https://archive.md/W7b4b>`__.
  
- Godoy, Jody. `“Equifax Data Breach Settlement Objectors Lose Appeal.” 
  <https://www.reuters.com/legal/litigation/equifax-data-breach-settlement-objectors-lose-appeal-2021-06-03/>`__ 
  *Reuters*, Thomson Reuters, 3 June 2021. `Archived <https://archive.md/frGxW>`__.
  
- `“2017 Equifax Data Breach.” 
  <https://en.wikipedia.org/wiki/2017_Equifax_data_breach>`__ 
  *Wikipedia*, Wikimedia Foundation, 25 Oct. 2021.
  
- `“Fourth Department of the General Staff Headquarters Department.” 
  <https://en.wikipedia.org/wiki/Fourth_Department_of_the_General_Staff_Headquarters_Department>`__ 
  *Wikipedia*, Wikimedia Foundation, 29 Oct. 2021.

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
   
.. [CA] “Allegation.” Cambridge Dictionary, 
   https://dictionary.cambridge.org/dictionary/english/allegation.
   `Archived <https://archive.md/3giqI>`__.
   
.. [CM] Chin, Monica. “On Top of Everything Else, Equifax Hackers Got 10 Million 
   Driver's Licenses.” *Mashable*, 11 Oct. 2017, 
   https://mashable.com/article/equifax-hackers-got-drivers-licenses.
   `Archived <https://archive.md/ubD10>`__.

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

.. [E] Inc., Equifax. “Equifax Announces Cybersecurity Incident Involving 
   Consumer Information.“ *PrNewsWire*, 7 Sept. 2017, 
   https://www.prnewswire.com/news-releases/equifax-announces-cybersecurity-incident-involving-consumer-information-300515960.html.
   `Archived <https://archive.md/MBXzP>`__.

.. [FA] Fifield, Anna. “China Rebuffs U.S. Charges of Cyberespionage over Equifax 
   Hack.” *The Washington Post*, WP Company, 20 Feb. 2020, 
   https://www.washingtonpost.com/world/asia_pacific/china-rebuffs-american-charges-of-cyber-espionage-over-equifax-hack/2020/02/11/b95fd932-4ca2-11ea-967b-e074d302c7d4_story.html.
   `Archived <https://archive.md/W7b4b>`__.
   
.. [G] Goodin, Dan. “Failure to Patch Two-Month-Old Bug Led to Massive Equifax 
   Breach.” *Ars Technica*, 13 Sept. 2017, 
   https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/.
   `Archived <https://archive.md/https://arstechnica.com/information-technology/2017/09/massive-equifax-breach-caused-by-failure-to-patch-two-month-old-bug/>`__.

.. [GS] Gallagher, Sean. “Equifax Hackers Stole Data for 200k Credit Cards from 
   Transaction History.” *Ars Technica*, 14 Sept. 2017, 
   https://arstechnica.com/information-technology/2017/09/equifax-hackers-stole-data-for-200k-credit-cards-from-transaction-history/.
   `Archived <https://archive.md/5Bkbc>`__.

.. [H] Hautala, Laura. “Equifax Ex-CEO: 'Both Human Error and Tech Failures' in 
   Massive Data Breach.” *CNET*, 2 Oct. 2017, 
   https://www.cnet.com/tech/services-and-software/equifax-ceo-data-breach-heres-what-went-wrong/.
   `Archived <https://archive.md/CuNmM>`__.

.. [HA] Hern, Alex. “Equifax Told to Inform Britons Whether They Are at Risk 
   after Data Breach.” *The Guardian*, Guardian News and Media, 8 Sept. 2017, 
   https://www.theguardian.com/technology/2017/sep/08/equifax-told-to-inform-britons-whether-they-are-at-risk-after-data-breach.
   `Archived <https://archive.md/a3PmP>`__.
   
.. [L] Lomas, Natasha. “Equifax Breach Disclosure Would Have Failed Europe's 
   Tough New Rules.” *TechCrunch*, 8 Sept. 2017, 
   https://techcrunch.com/2017/09/08/equifax-breach-disclosure-would-have-failed-europes-tough-new-rules/.
   `Archived <https://archive.md/ZtPUF>`__.

.. [M] Mathews, Lee. “Equifax Data Breach Impacts 143 Million Americans.” 
   *Forbes*, Forbes Magazine, 7 Sept. 2017,
   https://www.forbes.com/sites/leemathews/2017/09/07/equifax-data-breach-impacts-143-million-americans/?sh=16bb95ef356f.
   `Archived <https://archive.md/fo2um>`__.
   
.. [MM] “Equifax Data Breach Lawsuit.” *Morgan & Morgan*, 
    https://www.forthepeople.com/class-action-lawyers/equifax-data-breach-lawsuit/.
    `Archived <https://archive.md/GRPq3>`__.
   
.. [N] Ng, Alfred. “How the Equifax Hack Happened, and What Still Needs to Be 
   Done.” *CNET*, 7 Sept. 2018, 
   https://www.cnet.com/tech/services-and-software/equifaxs-hack-one-year-later-a-look-back-at-how-it-happened-and-whats-changed/.
   `Archived <https://archive.md/NVeDV>`__.

.. [N2] Ng, Alfred, and Musil, Steven. “Equifax Data Leak May Affect Nearly Half 
   the US Population.” *CNET*, 8 Sept. 2017, 
   https://www.cnet.com/tech/services-and-software/equifax-data-leak-hits-nearly-half-of-the-us-population/.
   `Archived <https://archive.md/dH7ei>`__.

.. [NL] Newman, Lily Hay. “How to Stop the Next Equifax-Style Megabreach-Or At 
   Least Slow It Down.” *Wired*, Conde Nast, 12 Sept. 2017, 
   https://www.wired.com/story/how-to-stop-breaches-equifax/.
   `Archived <https://archive.md/xL7vb>`__.
   
.. [RT] “Blaming Beijing: US Charges 4 Chinese Military Personnel over Massive Equifax Hack.” 
   *RT International*, 10 Feb. 2020,
   https://www.rt.com/usa/480536-chinese-military-hackers-equifax/.
   `Archived <https://archive.md/dEYcR>`__.

.. [S] Shepardson, David. “Equifax Failed to Patch Security Vulnerability in 
   March: Former CEO.” *Reuters*, Thomson Reuters, 2 Oct. 2017, 
   https://www.reuters.com/article/us-equifax-breach/equifax-failed-to-patch-security-vulnerability-in-march-former-ceo-idUSKCN1C71VY.
   `Archived <https://archive.md/MJ7zq>`__.

.. [T] Turcsányi, Gergő. “Deep Dive into the Equifax Breach and the Apache Struts 
   Vulnerability.” *Avatao*, 
   https://avatao.com/blog-deep-dive-into-the-equifax-breach-and-the-apache-struts-vulnerability/.
   `Archived <https://archive.md/LPy4G>`__.
   
.. [V] Viswanatha, Aruna, et al. “Four Members of China's Military Indicted Over 
   Massive Equifax Breach.” *The Wall Street Journal*, Dow Jones & Company, 10 
   Feb. 2020,
   https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824.
   `Archived 
   <https://web.archive.org/web/20211009220413/https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824>`__.
   
.. [VD] Volz, Dustin. “Prosecutors Said PLA's 54th Research Institute-Traditionally Focused 
   on Supporting Electronic Warfare Akin to Cyber Command as Opposed to Cyber Espionage-Was 
   behind the Hack, an Indication the Group's ‘Missions May Be Evolving," @EBKania Said. 
   Https://T.co/dB1bSAsE9h.” *Twitter*, 10 Feb. 2020, 
   https://twitter.com/dnvolz/status/1226983668222132225. 
   `Archived <https://archive.md/Tpwmu>`__.

.. [W] Whittaker, Zack. “Equifax Confirms Apache Struts Flaw It Failed to Patch 
   Was to Blame for Data Breach.” *ZDNet*, 13 Sept. 2017, 
   https://www.zdnet.com/article/equifax-confirms-apache-struts-flaw-it-failed-to-patch-was-to-blame-for-data-breach/.
   `Archived <https://archive.md/Qxreg>`__.
   
.. [WE] Weise, Elizabeth, and Nathan Bomey. “Equifax Breach Hit 2.5 Million More 
   Americans than First Believed.” *USA Today*, Gannett Satellite Information 
   Network, 2 Oct. 2017, 
   https://www.usatoday.com/story/tech/2017/10/02/equifax-breach-hit-2-5-million-more-americans-than-first-believed/725100001/.
   `Archived <https://archive.md/TfhLK>`__.
   
.. [WK] “2017 Equifax Data Breach.” *Wikipedia*, Wikimedia Foundation, 25 Oct. 
   2021, https://en.wikipedia.org/wiki/2017_Equifax_data_breach.
   
.. [WP] Wagenseil, Paul. “Equifax Data Breach Was China's Doing, According to the US Government.” 
   *Tom's Guide*, 10 Feb. 2020, 
   https://www.tomsguide.com/uk/news/equifax-hack-china-charges. 
   `Archived <https://archive.md/Pq3ut>`__.

.. URLs
.. _1.412 billion people: https://en.wikipedia.org/wiki/Demographics_of_China
.. _29 July 2017: https://www.prnewswire.com/news-releases/equifax-announces-cybersecurity-incident-involving-consumer-information-300515960.html
.. _2015 massive breach at the U.S. Office of Personnel Management: 
   https://web.archive.org/web/20201119114457/https://www.bloomberg.com/news/articles/2015-07-09/hackers-stole-government-data-on-25-7-million-people-u-s-says
.. _a months-old issue that Equifax knew about but failed to fix: https://www.cnet.com/news/equifax-ceo-data-breach-heres-what-went-wrong/
.. _accused China: https://www.cbc.ca/news/business/micosoft-exchange-hack-china-1.6108265
.. _Apache Struts: https://struts.apache.org/
.. _Apache Struts software: https://struts.apache.org/
.. _archive: https://web.archive.org/web/20210629150932/https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf
.. _CEO: https://archive.md/1aLaJ
.. _Chief Information Officer CIO of Equifax was sentenced to four months: 
   https://www.silicon.co.uk/e-regulation/legal/equifax-cio-jailed-insider-trading-268127
.. _Chinese Military Hackers Charged in Equifax Breach: https://www.fbi.gov/news/stories/chinese-hackers-charged-in-equifax-breach-021020
.. _Chinese Military Officers Hacked Equifax, Justice Department Say: 
   https://www.defenseone.com/technology/2020/02/chinese-military-officers-hacked-equifax-justice-department-says/163013/
.. _CIO and CSO: https://archive.md/qvmvJ
.. _CVE-2017-5638: https://www.cvedetails.com/cve/CVE-2017-5638/
.. _DOJ indictment: https://www.justice.gov/opa/press-release/file/1246891/download
.. _elite: https://www.thetimes.co.uk/article/chinese-armys-elite-hackers-steal-equifax-data-on-13m-britons-ld32rqjqq
.. _Equifax\: US charges four Chinese military officers over huge hack: 
   https://www.bbc.com/news/world-us-canada-51449778
.. _Equifax Lawsuit\: ‘Admin’ As Password At Time Of 2017 Breach: 
   https://www.forbes.com/sites/kateoflahertyuk/2019/10/20/equifax-lawsuit-reveals-terrible-security-practices-at-time-of-2017-breach/
.. _FBI most wanted: https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute
.. _FBI news article: https://www.fbi.gov/news/stories/chinese-hackers-charged-in-equifax-breach-021020
.. _filing: https://web.archive.org/web/20210112015402/http://securities.stanford.edu/filings-documents/1063/EI00_15/2019128_r01x_17CV03463.pdf
.. _Four Members of China's Military Indicted for Massive Equifax Breach: 
   https://www.wsj.com/articles/four-members-of-china-s-military-indicted-for-massive-equifax-breach-11581346824
.. _He thought wrong: https://abcnews.go.com/blogs/headlines/2014/07/russia-claims-alleged-hacker-was-kidnapped-by-us-agents
.. _indictment: https://www.justice.gov/opa/press-release/file/1246891/download
.. _Justice Department charges 4 members of Chinese military for massive Equifax hack: 
   https://www.cbsnews.com/news/equifax-hack-chinese-military-members-charged-department-of-justice/
.. _PDF: https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf
.. _press release: https://www.justice.gov/opa/pr/chinese-military-personnel-charged-computer-fraud-economic-espionage-and-wire-fraud-hacking
.. _Report\: Chinese Army Stole Over 13 Million British Citizens’ Personal Data:
   https://www.breitbart.com/europe/2020/02/17/equifax-hack-china-stole-13-million-peoples-data-in-the-uk/
.. _Roman Seleznev: https://en.wikipedia.org/wiki/Roman_Seleznev
.. _RT.com: https://www.rt.com/usa/480536-chinese-military-hackers-equifax/
.. _second most important army in the world in terms of budget: 
   https://en.wikipedia.org/wiki/List_of_countries_by_military_expenditures
.. _SecureWorld: https://www.secureworld.io/industry-news/equifax-hacker-indictment-10-fast-facts
.. _Silicon.co.uk: https://www.silicon.co.uk/security/cyberwar/us-charges-chinese-military-equifax-hack-331572
.. _Technical questions: ./technical_questions.rst
.. _"the Kremlin's foreign-language propaganda network": https://archive.md/CF3U6
.. _The US says the Chinese military hacked Equifax. Here’s how.: 
   https://www.technologyreview.com/2020/02/10/349004/the-us-says-the-chinese-military-hacked-equifax-heres-how/
.. _tom's guide: https://www.tomsguide.com/uk/news/equifax-hack-china-charges
.. _U.S. Charges Chinese Military Officers in 2017 Equifax Hacking: 
   https://archive.md/8EKZs
.. _US says China's military was behind 2017 Equifax hack that left personal information of 145 million Americans exposed:
   https://www.businessinsider.com/doj-china-pla-military-hackers-indicted-equifax-2017-breach-2020-2
.. _wanted poster put up online by the FBI: https://www.fbi.gov/wanted/cyber/chinese-pla-members-54th-research-institute
.. _What is the PLA, and why do feds believe they hacked Equifax?:
   https://www.ajc.com/news/what-the-pla-and-why-feds-believe-they-hacked-equifax/IwFZoHWI4ZEtptRldiD3mJ/
