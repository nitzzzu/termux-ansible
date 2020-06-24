- Install F-Droid
- Install Termux, Termux:Widget
- For Huawei phones: `Settings -> App launch -> Manage manually`
- Setup Termux for ansible access:

```
termux-setup-storage
termux-wake-lock
pkg upgrade
pkg install -y openssh python
echo 'qwerty' | passwd
sshd
```

- Copy rclone config in `files/.config/rclone/rclone.conf`
- Find IP of android phone: `ifconfig`
- Adapt `hosts.yml`
- Run script: `ansp -i hosts.yml playbook.yml`
- Enjoy termux scripts in the Termux:Widget