# IOChecker
The Informer Series: I/O Checker

I/O Checker is the first in a series of tools that DirectDefense will be releasing to the security community to assist with performing PCI (and general) security testing. Written by John Elliott, Principal Security Consultant for DirectDefense, I/O Checker assists PCI PA QSAs and security testers with tracking credit card data and file access during a card transaction on Windows systems.
  

Background:

 
 Forensics on images of host drives is the standard for finding data. I/O Checker is a new data tracking program designed to be used in conjunction with image based forensics. By leveraging both forensics and I/O Checker together a more comprehensive data analysis can be achieved during the PA QSA testing process.
  
 I/O Checker hooks into the Windows Kernel and catches all I/O activity. It then monitors for the “Search String” the user is looking for. I/O Checker and Image based Forensics together provide very thorough analysis.
  
▸I/O Checker is very quick to use. In a minute you can test in real-time where your critical transaction data is going.
▸I/O Checker catches all I/O not just what you can “image”. If you have many shared drives I/O Checker will catch data going out the shared drives, which may too voluminous to image.
▸I/O Checker catches data going to devices, not just files.
▸I/O Catcher has very low “false positives” because you control the I/O window of time you are examining. Forensics can produce so many “false positives” that you cannot use the results; whereas I/O Catcher is focused on a very small unit of time (your test time) so the chances of your search string matching some random I/O is very low.

 

When to use Forensics first:

 
▸Use Forensics to find historical data that I/O Catcher does not see because it is not being written to in real-time.
▸Use Forensic images to save a hosts “state” for future reference.
▸Combining forensics and I/O Checker will give you the best view into where all data is stored.

 
 At the end of your transaction, you will be presented with a series of logs and a HTML report to analyze and illustrate your findings.
  
 Additionally, I/O Checker has been written to also be configurable enough to be leveraged for any transaction functions you may need to monitor as the regex expression is tailored for your needs. One example, we have already used it for is tracking file access on an malware infected system to track an attackers behavior. The uses are limited to your imagination.
