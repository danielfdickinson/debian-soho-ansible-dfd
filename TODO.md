# To Do

* Fully configure sieve
* Configure spamassassin bayesian filer training
* Add backupmx role in a separate environment
* Refactor large roles to better separate concerns by splitting up the roles
* Check ansible-galaxy for potentially useful roles
* Clean up variable usage
* Make roles usable standalone
* Create simple collections for things like sogo and my separated IMAP / MX
setup
* Move SOGo authentication to HAProxy and use database password to access
IMAP/Submission (different pasword for SOGo than Dovecot)?
* What to do about encrypting data?
	* The problem is autorestarting in the case OVH needs to intervene (for
	example of the monitoring indicates non-responsiveness), which at least at
	first is a reboot.
