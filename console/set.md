# set

## Commands

- `set mgmtip <ip> <netmask> <gateway>`: Configure management interface IPv4
  - Example: `set mgmtip 192.168.1.10 255.255.255.0 192.168.1.1`
  - Notes: IPv4 only; `netmask` must be dotted-decimal (e.g. `255.255.255.0`)
- `set firewall <enable|disable>`: Enable/disable firewall
- `set radius <enable|disable>`: Enable/disable RADIUS
- `set tacplus <enable|disable>`: Enable/disable TACACS+

## Tip

You can also use `set help` / `set ?` to list available keys.

## Example: `set help` Output

```Text
> set help
Usage: set <key> ...
Available keys:
  mgmtip    - Set management IP address
  firewall  - Enable or disable firewall
  radius    - Enable or disable RADIUS authentication
  tacplus   - Enable or disable TACACS+ authentication
```