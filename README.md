# Cybersecurity
![](https://github.com/akchinSTC/Cybersecurity/blob/Week-9/Dec-01-2018%2020-20-09.gif)

HoneyPots deployed :
1. mhn-honeypot-2-shockpot
2. mhn-honeypot-1-dionaea
3. mhn-honeypot-4-cowrie

Issues encountered : 
Nothing much, had to do a password reset once, but the manual reset python script in MHN_HOME/server did not
have the dependencies installed from pip. Just installed and everything went ok.

Summary of the data collected: number of attacks, number of malware samples, etc:
Total # of attacks : 10508 in the past 24 hrs. 
Malware Samples Collected : 12
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	1425	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	1425	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	1259	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	1259	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:178.87.120.54	::ffff:10.138.0.3	::ffff:178.87.120.54	445	1347	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:178.87.120.54	::ffff:10.138.0.3	::ffff:178.87.120.54	445	2302	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:178.87.120.54	::ffff:10.138.0.3	::ffff:178.87.120.54	445	2302	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	4183	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	4183	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	2374	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	2374	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9
smb://::ffff:59.127.167.202	::ffff:10.138.0.3	::ffff:59.127.167.202	445	4141	284d28a084888eb4e5971d0edad8a877ff35b5dfcc8dd275314e4e6312595f3ca3194dece02111dc0f0c95ee217111f3602988c80326f91acdf79a1d1134ab3d	786ab616239814616642ba4438df78a9


Unresolved questions raised by the data collected :
The 2nd honey pot was created specifically to trap individuals going after the bash exploit  CVE-2014-6271. However after 
an entire week there were zero attacks against it, which makes me wonder why that is. First thought is that it was a niche and old exploit
that users / script kiddies dont want to attempt since it a time/benefit exercise for them. Exploiting newer vulnerabilities are worth
their time more. Second thought would be that operating systems have already patched this up to the point where going back to the
first, most machines are probably protected against this already
