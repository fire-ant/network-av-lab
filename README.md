Dante
=========

This repository serves as a basic example using ansible to configure the necessary extras to support networked AV, specifically Audniate Dante. 

Whilst not an exhaustive list it includes:
- disabling EEE
- disabling Green Ethernet
- enabling Jumbo Frames
- enabling IGMP snooping Globally
- enabling IGMP snooping per VLAN
- configuring VLANs
- Port to VLAN mapping
- setting QOS DSCP advanced mode
- configuring the correct DSCP markers to strict priority queues

Due to the nature of SMB switches such as the SG300 it is difficult to make it either idempotent or abstract the configurtation to data

Development will require a basic understandonf ansible and the Cisco SG300 CLI:

https://www.storagenetworks.com/documents/cisco/cisco-series300-manual.pdf



