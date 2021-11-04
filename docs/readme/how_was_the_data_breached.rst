==========================
How was the data breached?
==========================
`:star:`

  To go back to the main page about the 2017 Equifax data breach, click 
  `here`_.
  
----------

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
  occur, including [W]_:
  
  - the insecure network design which lacked sufficient segmentation [NL]_
  - potentially inadequate encryption of personally identifiable information 
    (PII) [G]_, and
  - ineffective breach detection mechanisms. [L]_

.. raw:: html

   <div align="center">
   <img src="https://camo.githubusercontent.com/4dbe1733c0ea00a63c6096fef006392d8544b2ef9e8947f3aafca507ba7837a1/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f313430302f302a46334476476b37755234583538613566" style="width:700px;height:500px;"/>
   <p><b>A chart from the <a href="https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf">GAO report</a>
      describing how Equifax was breached.</b></p>
   </div>

References
==========
.. [B] Bomey, Nathan. “How Chinese Military Hackers Allegedly Pulled off the 
   Equifax Data Breach, Stealing Data from 145 Million Americans.” *USA Today*, 
   Gannett Satellite Information Network, 10 Feb. 2020, 
   https://www.usatoday.com/story/tech/2020/02/10/2017-equifax-data-breach-chinese-military-hack/4712788002/.
   `Archived <https://archive.md/tMyN3>`__.
   
.. [G] Gallagher, Sean. “Equifax Hackers Stole Data for 200k Credit Cards from 
   Transaction History.” *Ars Technica*, 14 Sept. 2017, 
   https://arstechnica.com/information-technology/2017/09/equifax-hackers-stole-data-for-200k-credit-cards-from-transaction-history/.
   `Archived <https://archive.md/5Bkbc>`__.
   
.. [L] Lomas, Natasha. “Equifax Breach Disclosure Would Have Failed Europe's 
   Tough New Rules.” *TechCrunch*, 8 Sept. 2017, 
   https://techcrunch.com/2017/09/08/equifax-breach-disclosure-would-have-failed-europes-tough-new-rules/.
   `Archived <https://archive.md/ZtPUF>`__.

.. [M] Mathews, Lee. “Equifax Data Breach Impacts 143 Million Americans.” 
   *Forbes*, Forbes Magazine, 7 Sept. 2017,
   https://www.forbes.com/sites/leemathews/2017/09/07/equifax-data-breach-impacts-143-million-americans/?sh=16bb95ef356f.
   `Archived <https://archive.md/fo2um>`__.

.. [N] Ng, Alfred. “How the Equifax Hack Happened, and What Still Needs to Be 
   Done.” *CNET*, 7 Sept. 2018, 
   https://www.cnet.com/tech/services-and-software/equifaxs-hack-one-year-later-a-look-back-at-how-it-happened-and-whats-changed/.
   `Archived <https://archive.md/NVeDV>`__.
   
.. [NL] Newman, Lily Hay. “How to Stop the Next Equifax-Style Megabreach-Or At 
   Least Slow It Down.” *Wired*, Conde Nast, 12 Sept. 2017, 
   https://www.wired.com/story/how-to-stop-breaches-equifax/.
   `Archived <https://archive.md/xL7vb>`__.

.. [T] Turcsányi, Gergő. “Deep Dive into the Equifax Breach and the Apache Struts 
   Vulnerability.” *Avatao*, 
   https://avatao.com/blog-deep-dive-into-the-equifax-breach-and-the-apache-struts-vulnerability/.
   `Archived <https://archive.md/LPy4G>`__.

.. [W] “2017 Equifax Data Breach.” *Wikipedia*, Wikimedia Foundation, 25 Oct. 
   2021, https://en.wikipedia.org/wiki/2017_Equifax_data_breach.

.. URLs
.. _a months-old issue that Equifax knew about but failed to fix: https://www.cnet.com/news/equifax-ceo-data-breach-heres-what-went-wrong/
.. _archive: https://web.archive.org/web/20210629150932/https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf
.. _CVE-2017-5638: https://www.cvedetails.com/cve/CVE-2017-5638/
.. _here: https://github.com/raul23/equifax-data-breach/blob/main/README.rst#contents
.. _PDF: https://www.warren.senate.gov/imo/media/doc/2018.09.06%20GAO%20Equifax%20report.pdf
