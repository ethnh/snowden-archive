SNIPs of SIGINT
(U) Monthly Notes for June 2012
![img-0.jpeg](img-0.jpeg)

Entry tags: monthly notes

# Technical accomplishments 

## (U//FOUO) PITIED FOOL

- (TS//SI//REL) PITIEDFOOL is a suite of CNA tools I'm developing for use against file systems, initially focused on Windows. More information can be found on the $\underline{D S D}$ wiki, but it's a bit ugly at this point.
- (TS//SI//REL) Determined that it was a combination of the volume shadow copy and deleted entries in the shadow copy that were causing my recovery woes. As a result of the shadow copy having large chunks of MFT data in it, and much of these records still being mostly correct, recovery programs were able to reconstruct most of the system drive. I added functionality to PITIEDFOOL to overwrite the contents of the shadow copy on each partition encountered.
- (TS//SI//REL) Now that I was overwriting large chunks of data for every partition, I could no longer ignore the performance issues with writing to a disk one sector at a time. I refactored my code to overwrite in blocks configurable by a pre-processor definition and sped up execution about 15 -fold, with the possiblity of it going even faster with increased memory usage.
- (TS//SI//REL) After all this I tested PITIEDFOOL within FUZZYEBOLA and it worked flawlessly. I took a build of FUZZYEBOLA from last month, and without recompiling inserted the PITIEDFOOL binary with configuration details to execute it at a certain time. At that time I saw the process usage slightly increase (from $0 \%$ to around $2 \%$ ) and a few minutes later the system rebooted and didn't come back up. Running a file recovery tool over the entire drive yielded some files (from scraping headers) but nearly the entire contents of the drive were irrecoverable, and if it had been configured to securely wipe every sector on the drive after killing the MFT and VSS it wouldn't have been able to recover anything at all. Success!
- (U//FOUO) Documented my work.
(U//FOUO) PANT SPARTY
- (TS//SI//REL) PANT SPARTY is a backdoor in the SSH daemon for *NIX, based on OpenSSH portable. It allows a public key to be embedded in the sshd binary and will then always grant a root login shell if presented with the proper key pair for that key. In other words, it behaves as if the given key is in $-/ . s s h /$ authorized_keys.
- (TS//SI//REL) Currently DSD uses authorized_keys as a quick-and-easy method of persistence against certain *NIX targets. In most cases this
works, but it obviously isn't very stealthy and can run into problems if that file is deleted or the SSH configuration changes to not use it. The goal for this project was to provide the same level of persistence but embedded in the sshd binary itself (obviously, assuming root access, as before).

- (TS//SI//REL) By adding my own check in several key places within the SSH code I was able to grant authorization to a key embedded in the binary without too much trouble. The hard part came in granting that user root privileges even if the configuration specifically banned root login. That was achieved by setting a flag in the authorization context within the server that essentially said "this is our backdoor, let it happen, oh and stop logging also."
- (TS//SI//REL) Then I wanted to have it so if you provide a normal username as a login, it still grants you a root shell. SSH has a lot of checks to make sure you can't switch usernames in the middle of a login (go figure) so this was a bit tricky to bypass. Ultimately I was able to use the same flag as the previous step, and just had to put checks for it in other places.
- (TS//SI//REL) More fun was to be had when I wanted to allow an arbitrary username to be provided (i.e. one that doesn't exist on the system) while still allowing for root login. This led to all sorts of problems where I didn't even get a valid authorization context at all, and I couldn't manually call the C function to get one for root because the connection is a de-privileged child process, so I had to force-feed it a fake one for root. Of course, the force-fed hash for root doesn't match the entry in passwd, so I had to throw in another check there to return true if it's the backdoor. And there's all sorts of fun happening with pre-auth where I had to revert the authorization context back to its original value to postpone its processing (a standard authorization step in some cases) and then properly update it to root during the actual authorization step later on. Once I got this working, however, a user is able to run "ssh abcdefg@target" and the target's logs only show "Invalid username abcdefg" without the follow-on message of "Accepted publickey for root from 10.0.0.1 port 55000 ssh2". Presenting a valid username leads to the only logged output being that the public key check failed.
- (S//SI//REL) I set my new implant development PR on this project! My previous record was 3 days for DIRTYDEEDS, but I finished this in 2. Technically I had it working in a day, but it wasn't what I considered releasable, so I'll have to wait for some other opportunity to present itself so I can achieve the feat of an implant-in-a-day.


# Awards/Recognition 

(U//FOUO) Letter of Appreciation from
(U//FOUO) Letter of Appreciation from $\square$ Chief SUSLOC
(U//FOUO) SUSLOC coin

# Briefings and demonstrations given 

(S//REL) Briefed the U.S. Ambassador to Australia on my work on CNA/CNE and collaboration with TAO during my time at DSD.

## Meetings and briefings attended

(U) NSTR
(U) Weekly SUSLOC meetings

## Reports/papers/publications

(U) NSTR

## Training

(U) NSTR

## Miscellaneous

(U) New Zealand was incredible! I wish I'd had more time there, but I think I did pretty well. I saw a handful of LOTR sights, Mount Cook, a number of gorgeous lakes, snow-capped mountains everywhere. If you want pictures let me know and I'll shoot you the link.
(U) Tasmania was similarly awesome, and not just because I can now say "Yea, I've been to Tasmania," because, you know, it sounds cool.
(U) at the U.S. Embassy Independence Day Party!
(U//FOUO) My time at DSD came to a close in June, as my flight back is on 30 June ( 26 hours in an airplane, WOO!). I absolutely loved my time in Australia, both in terms of work and travel, but I'm also looking forward to returning to the land of Chick-fil-A, college athletics, BBQ pork, and real bacon. Oh, and good beer.
(U) THE BCS IS DEAD!!!!!! YESSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSS
SNIPs of SIGINT :: (U) Monthly Notes for June 2012

SSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSS
