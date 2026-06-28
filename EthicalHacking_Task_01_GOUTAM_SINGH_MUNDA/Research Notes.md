#Part A: Target Selection Choose one target:

Field	Details
Website Name	Kristu Jayanti University
URL	https://kristujayanti.edu.in

Reason for Choosing the Target	I selected my college website because I am a student of Kristu Jayanti University. It is a publicly accessible website that provides information about admissions, academics, events, and student services. Analyzing it helps me understand website structure and basic security concepts in an educational environment without performing any unauthorized activities.

#Part B: whois lookup

Field	Example (replace with your actual findings)
Domain Name	kristujayanti.edu.in
Registrar	National Internet Exchange of India
Registration Date	2025-05-28
Expiry Date	2023-05-28
Name Servers	ns01.trs-dns.com
ns01.trs-dns.net
ns10.trs-dns.info
ns10.trs-dns.org
Domain Status	
serverDeleteProhibited
serverTransferProhibited
serverUpdateProhibited

#Part C: dns enumeration 


#Part d : website technology
Technology	Identified
Web Server	Not publicly disclosed (behind a web server; exact server header is not exposed)
CMS	WordPress
Programming Language	PHP (likely, because WordPress is built on PHP)
JavaScript Framework / Library	jQuery
CDN	cloud front, bootstrap cdn, cdn js, cloudflare js, jsDelivr.


The analysis indicates that the Kristu Jayanti College website uses WordPress as its Content Management System (CMS). Since WordPress is built using PHP, the website is likely powered by PHP on the server side. The website also uses the jQuery JavaScript library to provide interactive features and improve the user experience. At the time of analysis, there was no publicly identifiable Content Delivery Network (CDN) detected. Some server-side technologies, such as the exact web server software, are not publicly exposed, which is a common security practice.


#Part e: http security header
: Image : 

| Security Header | Present (Yes/No) | Purpose |
|-----------------|------------------|---------|
| Content-Security-Policy (CSP) | Yes/No | Helps prevent Cross-Site Scripting (XSS) by controlling which resources the browser is allowed to load. |
| X-Frame-Options | Yes/No | Protects against clickjacking by preventing the website from being displayed inside unauthorized frames or iframes. |
| X-Content-Type-Options | Yes/No | Prevents browsers from MIME-type sniffing and forces them to use the declared content type. |
| Strict-Transport-Security (HSTS) | Yes/No | Forces browsers to use HTTPS connections, protecting against protocol downgrade and man-in-the-middle attacks. |
| Referrer-Policy | Yes/No | Controls how much referrer information is shared when users navigate to another website. |

Security Header	Present (Yes/No)	Purpose
Content-Security-Policy (CSP)	Yes	Prevents Cross-Site Scripting (XSS) attacks by restricting allowed resources.
X-Frame-Options	Yes	Protects against clickjacking attacks.
X-Content-Type-Options	Yes	Prevents MIME-type sniffing by browsers.
Strict-Transport-Security (HSTS)	Yes	Ensures all future connections use HTTPS.
Referrer-Policy	No	Controls what referrer information is sent to other websites.


#Part F: robots.txt & sitemap analysis
![Nmap Scan](SCREENSHOTS/1(10).png)

1. Does the website have a robots.txt file?
Answer: Yes. The website has a robots.txt file located at the root of the domain. This file provides instructions to search engine crawlers about which parts of the website they are allowed or not allowed to crawl. It may also include the location of the website's XML sitemap. 

2. Does the website have a sitemap.xml file?
Answer: Yes. The website provides a sitemap (or a sitemap index) that lists URLs intended for search engines to discover and index. XML sitemaps help search engines find important pages more efficiently. 

3. What information can be learned from these files?
From robots.txt
The robots.txt file can provide information such as:
•	Which directories or pages are allowed for crawling. 
•	Which directories or pages are disallowed. 
•	The location of the XML sitemap. 
•	Instructions intended for search engine crawlers. 
![Nmap Scan](SCREENSHOTS/1(11).png)
From sitemap.xml
The sitemap.xml file can provide information such as:
•	A list of website URLs. 
•	Important pages that the website wants search engines to index. 
•	The website's overall structure. 
•	Metadata such as the last modification date for pages (if included).

#Part G: Reconnaissance Report


#Website Reconnaissance Report

Reason for Selection:
The website was selected because it is the official website of my college and is publicly accessible. The objective of this reconnaissance exercise was to gather publicly available information for educational purposes without performing any intrusive or unauthorized activities.

The reconnaissance phase demonstrated how much useful information can be collected from publicly available sources without performing any intrusive actions. By examining WHOIS records, DNS information, website technologies, HTTP security headers, and search engine configuration files, it is possible to understand a website's infrastructure and security posture. This exercise highlighted the importance of passive information gathering in cybersecurity, as it helps security professionals identify technologies, configurations, and potential areas that may require further review while remaining within ethical and legal boundaries. I also learned how tools such as WHOIS lookup services, DNS lookup utilities, Wappalyzer, and SecurityHeaders.com can be used to collect valuable information for security assessments. Overall, the reconnaissance phase is an essential first step in cybersecurity because it provides a better understanding of the target environment and supports informed security analysis without disrupting normal website operations.
