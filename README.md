this script uses mutt for sending mail.
so there are serveral steps to do before it works on ubuntu
	1. install mutt and msmtp
		sudo apt-get install mutt
		sudo apt-get install msmtp
	2. edit ~/.muttrc
		set sendmail="/usr/bin/msmtp"
		set use_from=yes 
		set realname=YOUR_NAME
		set from=YOUR_ADDRESS
		set envelope_from=yes
	3. edit ~/.msmtprc
		account default
		host SMTP_SERVER
		from YOUR_ADDRESS
		auth plain
		user YOUR_NAME
		password ******
		logfile ~/.msmtp.log
	4. before using sendMail script, please read explaination at the beginning of the file. ENJOY IT.
