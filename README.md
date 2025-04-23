# Podman Quadlets

Put the `.container` files in:
```sh
$HOME/.config/containers/systemd/
```

Podman quadlet must be controlled from systemd.
```sh
# Everytime podlet is edited it must be reloaded to work.
systemctl --user daemon-reload
# Quadlet start stop. To permanently stop .container file must be delete.
systemctl --user start syncthing.service
systemctl --user stop syncthing.service
```
