# nvidia-laptop-power-cfg

This repo contains configuration files (and an archlinux package) to properly configure the nvidia power management.

## Installation

```sh
git clone https://gitlab.com/asus-linux/nvidia-laptop-power-cfg.git
makepkg -sfi
```

## Additional steps

If you haven't done already enable nvidia services:

```sh
sudo systemctl enable nvidia-suspend nvidia-resume nvidia-hibernate
sudo systemctl enable --now nvidia-powerd
sudo systemctl enable nvidia-suspend-then-hibernate.service
```
