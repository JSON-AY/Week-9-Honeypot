# Week-9-Honeypot

[Honeypot Attack Menu Photo](https://imgur.com/a/3CAuFBj)

[Honeypot Attack Map Photo](https://imgur.com/a/Eq8N5Fk)

[Nmap Scan of Honeypot Photo](https://imgur.com/a/tvhWb5d)

Which Honeypot(s) you deployed: I deployed the Dionaea honeypot with Ubuntu 14.04

Any issues you encountered: I had absolutely no luck with getting the Google Cloud Engine steps to work. I tried deploying three different projects and was unable to get the web page to load the admin sign-in page. The attack map would load and state that it was connected to the back end server, but I was never able to get the admin sign-in page to come up. I even tried adding on ports to the end of the IP Address in the URL but the only port that would do anything was 3000, which was the attack map.

I use Digital Ocean for personal projects every once in awhile so, I decided to give the setup a go by creating a new droplet. Lo and behold, the setup worked flawlessly and I was able to setup my admin box and honeypot without any snags. I have no idea where my steps may have been failing on the gcloud setup because, the exact same steps on my digital ocean server worked just fine.  ¯\_(ツ)_/¯

A summary of the data collected: number of attacks, number of malware samples, etc...: Since I deployed the Dionaea honeypot, the majority of the attacks I recevied appeared to be port scans to narrow down where vulnerabilities may lie with the service ports that my server had open. I had a total of over 18,000 attacks that I got during the course of an 18 hour honeypot deployment (roughly 1,000 attacks per hour). Since the Dionaea honeypot is built to have specific ports open, the majority of the attacks/vuln scans against the honeypot were as follows: SMB, HTTP, FTP, TFTP, MSSQL, MySQL, SIP (VOIP).

I've attached the exported json file that contains the details for these attacks. 

Any unresolved questions raised by the data collected: n/a
