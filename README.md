# AppArmor Profiles for Arch Linux

This repo contains apparmor profiles for Arch Linux and which are not available in the [apparmor](https://www.archlinux.org/packages/community/x86_64/apparmor/) package on Arch Linux. For instructions on how to install and configure apparmor read the [wiki article](https://wiki.archlinux.org/index.php/AppArmor).

## Supported profiles

| Profile                           | Program description              | Notes                                     |
| ----------------------------------|----------------------------------|-------------------------------------------|
| usr.bin.weechat                   | weechat apparmor profile         | /exec is disallowed, not all plugins work |
| usr.bin.houndd                    | hound daemon                     | none                                      |
| usr.bin.prometheus-node-exporter  | prometheus-node-exporter daemon  | none                                      |
| usr.bin.taskd                     | taskwarrior daemon               | none                                      |
| usr.bin.nginx                     | nginx webserver                  | webroot is defined as /srv/               |
| usr.bin.zathura                   | zathura pdf viewer               | whole $HOME is readable                   |
| usr.bin.grafana-server            | grafana server                   | none                                      |
| usr.bin.transmission-daemon       | transmission                     | /mnt/download as download directory       |
