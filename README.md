# shutdown-after-crashed

A systemd service that shuts down the system next time it boots after a crash for Arch Linux.

## Why?

I have a server that has a wake-on-lan feature. But if it goes down due to a breaker trip, WOL won't come back on without a reboot after a power outage. This is a workaround for that. If automatic restart after power outage is enabled, the server will automatically restart after the breaker trip. and then, this service was used to shut down the server. This left WOL running.

## Usage

1. Clone this repository.
1. Run `makepkg -si`.
1. Run `sudo systemctl enable --now shutdown-after-crashed` to enable the service.
1. Edit settings for your motherboard to power on after power loss.

## License

MIT

## Contributing

Feel free to open an issue or a pull request.
