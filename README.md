## Install:
SSH into you pi and run:
```
cd ~
wget -O - https://raw.githubusercontent.com/Zeanon/Tec-Tester/main/install.sh | bash
```

then add this to your moonraker.conf:
```
[update_manager tec-tester]
type: git_repo
channel: dev
path: ~/tec-tester
origin: https://github.com/Zeanon/Tec-Tester.git
managed_services: klipper
primary_branch: main
install_script: install.sh
```
