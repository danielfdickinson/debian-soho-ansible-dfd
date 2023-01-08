# To Do

* Only install/configure fail2ban as a dependency not as a separate task
	* E.g. should not be in the playbook, rather only triggered
* Likewise UFW (except should not be in a task list for a service / package)
* Configure backups
* Fully configure sieve
* Configure spamassassin bayesian filter training
* Add backupmx role in a separate environment
* Refactor large roles to better separate concerns by splitting up the roles
* Check ansible-galaxy for potentially useful roles
* Clean up variable usage
* Make roles usable standalone
* Create simple collections for things like sogo and my separated IMAP / MX
setup (maybe)
* What to do about encrypting data?
	* The problem is autorestarting in the case OVH needs to intervene (for
	example of the monitoring indicates non-responsiveness), which at least at
	first is a reboot.
