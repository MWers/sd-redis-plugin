# Redis Plugin for ServerDensity

## Installation

1. Copy `Redis.py` to your `sd-agent` plugins directory

    ```bash
    $ grep plugin_directory /etc/sd-agent/config.cfg
    # => plugin_directory: /opt/sd-agent/plugins

    $ cp Redis.py /opt/sd-agent/plugins
    ```

1. Install Redis python package

    ```bash
    $ pip install -r requirements.txt
    ```

1. Add config to `/etc/sd-agent/config.cfg` (optional)

    ```bash
    # Redis
    redis_host: localhost
    redis_port: 6379
    redis_password:
    ```

1. Restart `sd-agent`

    ```bash
    $ service sd-agent restart
    ```

## Credits

This plugin borrows heavily from the no-longer-supported Redis Plugin for ServerDensity from [cloudControl](https://github.com/cloudControl).

