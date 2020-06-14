# delayed-hibernation (deprecated)
Systemd service to hibernate suspended system after an hour.

After installation enable it with sudo systemctl enable suspend-to-hibernate.service

# update
Modern systemd has built-in support for delayed hibernation.
To trigger it, use:

`systemctl suspend-then-hibernate`

You can specify the timeout in `/etc/systemd/sleep.conf`, e.g.

`HibernateDelaySec=30min`
