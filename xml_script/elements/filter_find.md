---
description: Defines the find(f). It has a start tag <find> or <f>
---

# \<find>

## Attribute

<table><thead><tr><th width="150">Attribute</th><th width="215">Description</th><th width="157">Type</th><th>Default (* must have)</th></tr></thead><tbody><tr><td>id</td><td>Specifies a unique id for an element</td><td>Interger</td><td></td></tr><tr><td>name</td><td>refer to wireshark filter function, but less item</td><td>String</td><td>*</td></tr><tr><td>relation</td><td>Equal</td><td>==</td><td>*</td></tr><tr><td>content</td><td>content of name, could be empty</td><td>String</td><td>*</td></tr></tbody></table>

### Attribute -name

<table><thead><tr><th width="151.32440213813035">name</th><th width="177">type</th><th width="166.61725067385444">Description</th><th width="156">Example</th></tr></thead><tbody><tr><td>eth.addr</td><td></td><td></td><td></td></tr><tr><td>ip.addr</td><td>IPv4 address</td><td>Source or Destination Address</td><td>ip.addr == 8.8.8.8</td></tr><tr><td>ip.src</td><td>IPv4 address</td><td>Source Address</td><td>ip.src == 8.8.8.8</td></tr><tr><td>ip.dst</td><td>IPv4 address</td><td>Destination Address</td><td>ip.dst == 8.8.8.8</td></tr><tr><td>ip.proto</td><td>Unsigned integer, 1 byte</td><td>Protocol</td><td>ip.proto == 6 (TCP)</td></tr><tr><td>tcp.port</td><td>Unsigned integer, 2 bytes</td><td>Source or Destination Port</td><td>tcp.port == 443</td></tr><tr><td>tcp.srcport</td><td>Unsigned integer, 2 bytes</td><td>Source Port</td><td>tcp.srcport == 443</td></tr><tr><td>tcp.dstport</td><td>Unsigned integer, 2 bytes</td><td>Destination Port</td><td>tcp.dstport == 443</td></tr><tr><td>udp.port</td><td>Unsigned integer, 2 bytes</td><td>Source or Destination Port</td><td>udp.port == 53</td></tr><tr><td>udp.srcport</td><td>Unsigned integer, 2 bytes</td><td>Source Port</td><td>udp.srcport == 53</td></tr><tr><td>udp.dstport</td><td>Unsigned integer, 2 bytes</td><td>Destination Port</td><td>udp.dstport == 53</td></tr></tbody></table>

## Example

```xml
<filter id="1">
  <or>
    <find id="1" name="ip.addr" relation="==" content="8.8.8.8" />
    <find id="2" name="ip.addr" relation="==" content="2.2.2.2" />
  </or>
</filter>
```

```xml
<filter id="1">
  <or>
    <f n="ip.addr" r="==" c="8.8.8.8" />
    <f n="ip.addr" r="==" c="2.2.2.2" />
  </or>
</filter>
```
