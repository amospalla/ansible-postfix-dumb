# ansible-postfix-dumb
* * *

## Description

Installs and set up postfix to allow sending email through an external authenticated account.

By default it allows sending email only to local accounts so /etc/aliases needs to be feed with real external accounts. This behaviour can be disabled setting _postfix_dumb_only_local_accounts_ to False.

## Variables

Mandatory:

- _postfix_dumb_email_aliases_: dictionary for setting /etc/aliases file. Key/value correspond to user: destination.
- _postfix_dumb_relay_host_: remote server host.
- _postfix_dumb_relay_port_: remote server port.
-_postfix_dumb_relay_username_: remote account username.
-_postfix_dumb_relay_password_: remote account password.

Optional:
- _postfix_dumb_hostname_: hostname to use on main.cf instead of {{ ansible_inventory }}.
