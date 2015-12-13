Ansible role for set up Postix to send mail through an external authenticated account only.

This role sets up Postfix to use an authenticated smtp user on another e-mail server. It only allows delivering mail to local accounts.

Variables:

postfix_ea_enable: boolean (determines if role is applied to host)

postfix_ea_relayhost:
postfix_ea_relayhostport:
postfix_ea_username:
postfix_ea_password:
postfix_ea_header_checks_only_local_users: boolean (only allow to send email to local accounts, who can then be mapped to something through aliases file)

postfix_ea_email_aliases:
  localuser1: user1@domain1
  localuser2: user2@domain2
