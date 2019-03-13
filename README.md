# ansible_first_settings_role
Role for ansible,which create user and get him ssh access from ansible server.

## Algorithm:
1. Create user "ansible" on remote client
2. Set authorized key of server taken from file
3. Give correct rights to privet key on server
4. Fetch privet key from ansible server
5. Add user ansible to /etc/sudoers
6. Change AllowUsers in /etc/ssh/sshd_config
7. Restart sshd by notify

## Files:
1. handlers/main.yml - hendler for restart sshd
2. tasks/main.yml - main tasks file
3. vars/main.yml - files with variables

