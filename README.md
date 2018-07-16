# Plesk-Server-Notes
Just some Plesk-Server-Notes to show up how to set up a Ubuntu 16.04.4 Server by HostEurope.de by a example...

<br>

Pakets to install on the command line:  
- mc
- rkhunter filerights
- chkrootkit
- rkhunter

<br>

SSH:  
I would definitely recommend using RSA keys for SSH, that is what I use for my personal SSH server. I personally generate 4096-bit RSA keys, so I would recommend that, as well, just for extra security. Usually the default is 2048. It's also important to remember to disabled passwords,  
"PasswordAuthentication no" in the sshd_config, so the SSH server requires keys and does not allow passwords.  
https://support.plesk.com/hc/en-us/articles/115000065489-How-to-set-up-SSH-keys  

<br>

Fail2ban for Joomla!:  
https://www.andrehotzler.de/en/blog/technology/63-protect-joomla-login-with-fail2ban.html  

<br>

Addininat Pakets to install on command line:  
- drweb
- clamav

<br>

Sell domains:  
Just some more links on domain name speculation:  
https://auctions.godaddy.com/  
https://sedo.com/de/  

<br>

Escrow Service for domain sell:  
https://www.payoneer.com/escrow/domain-names/  
And another escrow website is https://www.escrow.com/  

<br>
