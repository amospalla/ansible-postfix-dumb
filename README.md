Ansible role for set up Postix to send mail through an external authenticated account only.

This role sets up Postfix to use an authenticated smtp user on another e-mail server. It only allows delivering mail to local accounts.

Variables:

relayhost:
relayhostport:
username:
password:
header_checks_only_local_users:

email_aliases:
  localuser1: user1@domain1
  localuser2: user2@domain2
