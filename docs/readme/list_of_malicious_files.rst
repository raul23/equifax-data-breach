====================================================================
List of malicious files and web shells allegedly used by the hackers
====================================================================
`:star:`

  To go back to the main page about the 2017 Equifax data breach, click 
  `here`_.
  
----------

`:information_source:`

  This list is compiled from the United States Department of Justice 
  (DOJ) `indictment`_ that was unsealed on February 10, 2020.
  
**Malicious files:**

1. ``jndi.txt`` [DOJ2]_ (paragraph 14.e, page 8)
2. ``abc.txt`` [DOJ2]_ (paragraph 14.l, page 10)

**Web shells:**

1. ``Jquery1.3.2.inin.jsp`` [DOJ2]_ (paragraph 14.e, page 8)
2. ``css.jsp`` which was allegedly used for:
  
   - downloading the ``abc.txt`` file from the Taiwan Server
  
     [DOJ2]_ (paragraph 14.l, page 10)
   - deleting an archive from Equifax's network in an effort to 
     conceal the theft of Equifax data
    
     [DOJ2]_ (paragraph 14.n, page 11)
3. ``ss.jsp`` is a substantively identical web shell to ``css.jsp``.

   [DOJ2]_ (paragraph 14.l, page 10)
4. ``boxover.jsp`` which was allegedly used to query an Equifax 
   database table and store the results in output files.
   
   [DOJ2]_ (paragraph 14.n, page 10)
5. ``six.jsp`` which was allegedly used to issue unauthorized SQL 
   commands to one of Equifax's back-end databases
    
   [DOJ2]_ (paragraph 14.o, page 11)

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

.. URLs
.. _here: https://github.com/raul23/equifax-data-breach/blob/main/README.rst
.. _indictment: https://www.justice.gov/opa/press-release/file/1246891/download
