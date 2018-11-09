## Install

#### Ubuntu:
`sudo apt-get install conky`

#### Centos:
`yum install -y epel-release`

`yum install -y conky`

## Configuration

By default conky uses a configuration file located:
`~/.conkyrc`

You can print out an example configuration:
`conky -C`

## Autostart

In `/etc/conky/conky.conf`:

```
conky.config = {
    background = true,
}
```

If you use a graphical desktop environment and wish to use a conky.desktop file for autostarting edit `~/.config/autostart/conky.desktop`:

```
[Desktop Entry]
Type=Application
Name=conky
Exec=conky --daemonize --pause=5
StartupNotify=false
Terminal=false
```
