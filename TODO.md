# To Do

## For first deploy to 'production'

* Add backupmx role in a separate environment
* Enable `deploy-test` password protected static web host vhost
* Make sure we have wanted headers on static web hosts.

## Soon after

* Configure backups on BHS (once ready to switch BHS to new instances)

## Later

* Fully configure sieve
* Configure spamassassin bayesian filter training
* Refactor large roles to better separate concerns by splitting up the roles
* Check ansible-galaxy for potentially useful roles
* Create collections for things like sogo and my separated IMAP / MX
setup
* What to do about encrypting data?
	* An issue is autorestarting in the case OVH needs to intervene (for
	example if the monitoring indicates non-responsiveness), which at least at
	first is a reboot.
* Make mail/groupware users and aliases PostgreSQL backed
	* Use a separate repo for holding the demo users and aliases.
	* Make sure I have a reasonable way of adding/removing uses and aliases from
		the database.
