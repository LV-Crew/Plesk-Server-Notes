# Plesk-Server-Notes
Just some Plesk-Server-Notes to show up how to set up a Ubuntu 16.04.4 Server by HostEurope.de by a example...  

<br>

Way to go:  
- Note all changes down for documentation... (...you can make a commit to get them here included! ;-) )  
- Renember to make always backups of changed files to have them again e.g. for migration.  
- Renember to first try to solve issues with Plesk and Plesk-Extensions - so you have it easier later to migrate with Plesk Migrator!  

<br>

Setup for the Plesk-only Part & Extensions:  
This is a own documentation...  
https://github.com/LV-Crew/Plesk-Notes  

<br>

SU for system users:  
Command Line: usermod -aG sudo -username-

<br>

Pakets to install on the command line:  
- mc
- 'rkhunter filerights'
- chkrootkit
- rkhunter

<br>

Set up Host Name:  
Follows...  
Files to back up: hostname_vps, hostname_vps.service, my.hosts  

<br>

SSH:  
I would definitely recommend using RSA keys for SSH, that is what I use for my personal SSH server. I personally generate 4096-bit RSA keys, so I would recommend that, as well, just for extra security. Usually the default is 2048. It's also important to remember to disabled passwords,  
"PasswordAuthentication no" in the sshd_config, so the SSH server requires keys and does not allow passwords.  
https://support.plesk.com/hc/en-us/articles/115000065489-How-to-set-up-SSH-keys  
Files to back up: sshd_config + User Keys  

<br>

.htpasswd to saver place:  
Follows...  
The old location is here:  
/var/www/vhosts/-domain-/httpdocs/administrator/  
The new location is here:  
/var/www/vhosts/-domain-/private/  
Files to back up: .htaccess, .htpasswd  

<br>

error-file to saver place:  
We also move the Joomla log files to a new directory to make it more secure. Because it contains user IP addresses, it is "sensitive" and should be protected for data privacy reasons.  
The old location is here:  
/var/www/vhosts/-domain-/httpdocs/administrator/logs/error.php  
The new location is here:  
/var/www/vhosts/-domain-/logs/joomla/error.php  


<br>

Fail2ban for Joomla!: (Not done yet!)  
https://www.andrehotzler.de/en/blog/technology/63-protect-joomla-login-with-fail2ban.html  
Files to back up: ...  

<br>

Host on Tor: (Not done yet!)
Files to back up: ...  

<br>

Addinional Pakets to install on command line: (Not done yet!)  
- drweb
- clamav
Files to back up: ...  

<br>

Sell domains: (domain name speculation)  
Add parking website from e.g. https://www.domainholder.io/.  
Example: https://y-lounge.com/  

<br>

Advertise domains: (domain name speculation)  
...always just suggest advertising domain names on as many sites as possible...  
...there is no any one special website for it, everyone just uses all of them to increase their chances to find someone they can negotiate a good price with.  
https://www.domainholder.io/  
https://auctions.godaddy.com/  
https://sedo.com/de/  

<br>

Escrow Service for domain sell:  
https://www.payoneer.com/escrow/domain-names/  
https://www.escrow.com/  
