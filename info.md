# linksys_ap

_Due to [ADR0004](https://github.com/home-assistant/architecture/blob/master/adr/0004-webscraping.md) this integration was removed from [Home Assistant](https://github.com/home-assistant/home-assistant/tree/0.99.0) with version 0.100, and are now republished here._

⚠️ This integration scrapes a website to get the information!
⚠️ There are no one actively maintaining this repository.

The linksys_ap platform offers presence detection by looking at connected devices to a Linksys based access point.

It was tested with a LAPAC1750 AC1750 Dual Band Access Point.

## Example configuration.yaml

```yaml
device_tracker:
  - platform: linksys_ap
    host: 192.168.1.1
    username: YOUR_USERNAME
    password: YOUR_PASSWORD
```

### Configuration options

Key | Type | Required | Description
-- | -- | -- | --
`host` | `string` | `True` | The hostname or IP address of your access point, e.g., 192.168.1.1.
`username` | `string` | `True` | The username of an user with administrative privileges (read-only is sufficient).
`password` | `string` | `True` | The password for your given admin account.
`verify_ssl` | `boolean` | `False` | Verify SSL certificate for HTTPS request.