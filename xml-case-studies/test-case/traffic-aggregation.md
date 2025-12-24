# Traffic Aggregation

This case study shows how to aggregate traffic from multiple input ports to a single output port.

## Flow

![Traffic Aggregation Flow](/.gitbook/assets/traffic-aggregation.svg)

## GRISM XML Script

```xml
<run>
    <chain>
        <in>S1.1</in>
        <out>S2.1</out>
    </chain>
    <chain>
        <in>S1.2</in>
        <out>S2.1</out>
    </chain>
</run>
```

## Behavior

- **Inputs**: Packets enter from ports `S1.1` and `S1.2`.
- **Aggregation**: Both chains forward traffic to the same output port `S2.1`.
- **Result**: Traffic from multiple sources is merged onto a single egress port.
