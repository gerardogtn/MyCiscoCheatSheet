# Configuring Routing Protocols.

## Default route
`(config)# ip route 0.0.0.0 0.0.0.0 $INTERFACE$ $IP$`

## RIPv2
`(config)# router rip`

`(config-router)# version 2`

### Passive interface
Passive interfaces are used to avoid sending packets with dynamic routing protocol information to interfaces that are not connected to other routers.

`(config)# router rip`

`(config-router)# passive-interface $INTERFACE$`

Here `$INTERFACES$` is the interface of the router that is not connected to another router (or to a router that has static routing configuration).

### No summarization
`(config)# no auto-summary`

### Share default route information
`default-information originate`

## RIPng
`(config)# interface $INTERFACE$`
`(config-if)# ipv6 rip RIP-AS enable`
`(config-if)# no shutdown`
