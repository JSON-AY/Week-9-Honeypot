# Week-9-Honeypot

[HoneyPot](https://imgur.com/a/3CAuFBj)

Which Honeypot(s) you deployed: I deployed the Dionaea honeypot with Ubuntu 14.04

Any issues you encountered: I had absolutely no luck with getting the Google Cloud Engine steps to work. I tried deploying three different projects and was unable to get the web page to load the admin sign-in page. The attack map would load and state that it was connected to the back end server, but I was never able to get the admin sign-in page to come up. I even tried adding on ports to the end of the ip address in the URL but the only port that would do anything was 3000, which was the attack map.

I use Digital Ocean for personal projects every once in awhile so, I decided to give the setup a go by creating a new droplet. Lo and behold, the setup worked flawlessly and I was able to setup my admin box and honeypot without any snags. I have no idea where my steps may have been failing on the gcloud setup, because the exact same steps on my digital ocean server worked just fine. ¯\_(ツ)_/¯

A summary of the data collected: number of attacks, number of malware samples, etc.

Any unresolved questions raised by the data collected



Additionally, include a json export of the data you collected in the repo, instructions for which can be found in the next section.
