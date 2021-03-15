# Role pam sshd login mail

configure pam to send a mail on every successful login through ssh.
Notifications are only sent once a day for every combination of username and ip.

## Parameters

| name            | default                  | description                                           |
|-----------------|--------------------------|-------------------------------------------------------|
| `recipient`     | `root@localhost`         | Recipient of notification email                       |
| `subject`       | `SSH Login: $PAM_USER`   | Subject of notification email                         |
| `remember_file` | `/tmp/pam_mail_on_login` | File to keep the username/ip combinations for the day |
| `do_remember`   | `true`                   | Whether to remember logins for a day                  |
