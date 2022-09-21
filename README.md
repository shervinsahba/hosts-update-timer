# hosts-update-timer

This installs a systemd timer and service, `hosts-update`, that periodically updates the `/etc/hosts/` file with [StevenBlack's hosts repository](https://github.com/StevenBlack/hosts). 

By default, the timer runs weekly and provides the unified+fakenews hosts. The files are copied to `/etc/systemd/system`. If you'd like to set a different update period or include some of StevenBlack's other lists, edit the timer and service files prior to running setup.

```
git clone https://github.com/shervinsahba/hosts-update-timer
cd hosts-update-timer && ./setup
```
