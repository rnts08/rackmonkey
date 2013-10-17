rackmonkey
==========

Rackmonkey fork for improvements and new features.

Feature wish-list
-------------------------

- [x] Raw paste from cli-output in hardware-devices, for example 'show chassis hardware' 
      without styling (enclose hardware and device Notes with pre-tags).
- [ ] IP-address field on devices
- [ ] OOB-management clickable link/ip-address field (ILOM/IPMI)
- [ ] Ports on switches and routers, with descriptions and 'type' (nic|transit|peering|core|access)
- [ ] Link ports from switches and routers with devices (depending on hardware/device-type,
      for example link access-switch-ports to core-switch-ports, access-switch-port with server-
      nics).

      This requires a 1:N relationship with device -> ports, and the ports will have a 1:1 
      relationship with another port. Some database-work is required for this as well:
        * Ports: port_id, device_id, port_type_id, description, connected_to_port_id, ... 
        * PortTypes: port_type_id, description
- [ ] Fields for monitoring URLs
- [ ] New device-roles with special meaning (Server-Chassis, Server-Blade) where
      a server-chassi is linked to server-blades (parent->child, 1:N relationships).

More to come!


