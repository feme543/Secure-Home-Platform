# Network Design

## Overview
The network is segmented into multiple security zones to reduce risk and prevent lateral movement.

## Network Zones
- ADMIN: Trusted devices used for system administration and management
- SERVERS: Hosts production services such as media servers, NVR, and logging platforms
- IOT: Untrusted devices including cameras and smart devices

## Traffic Policy
- ADMIN can access SERVERS for management purposes
- IOT devices can only communicate with designated server endpoints
- East-west traffic between zones is restricted by firewall rules
