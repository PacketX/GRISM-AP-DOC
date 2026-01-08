# Global Commands

- `help` / `?`: Show command help
- `show`: Show current configuration/status
- `reboot`: Reboot
- `shutdown`: Power off
- `exit` / `quit`: Exit

## Example: `?` Output

```Text
> ?
Available commands:
  set <key> ...          - Set a configuration parameter
  reset <key>            - Reset a configuration parameter to default
  reboot                 - Reboot the system
  shutdown               - Shutdown the system
  show                   - Show current configuration
  help, ?                - Show this help message
  exit, quit             - Exit the console
```

## Example: `show` Output

```Text
> show
MGMT IP: 192.168.1.64, Netmask: 255.255.255.0, Gateway:
RADIUS Enable: false
TACACS+ Enable: false
Firewall Enable: true
Allow IP List:
```

