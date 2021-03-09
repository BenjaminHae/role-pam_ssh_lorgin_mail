# Role pam sshd login mail

configure pam to send a mail on every successful login through ssh

## Parameters

| name        | default                | description                     |
|-------------|------------------------|---------------------------------|
| `recipient` | `root@localhost`       | Recipient of notification email |
| `subject`   | `SSH Login: $PAM_USER` | Subject of notification email   |
