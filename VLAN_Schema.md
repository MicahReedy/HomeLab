# The Home Cloud VLAN Schema

## Attributions

### Purpose

This document is to delineate the overal VLAN schema in use in the Home Cloud Lab

### Authorship

Micah Reedy - Sole Contributor

### Date of Publication

30-04-2026 at 19:40


## General Network Division Information and Rationale

The Home Cloud Lab is subnetted such that the second octet (X.100.X.X) represents the primary segment which the traffic belongs to.

## Home Cloud Lab Supernet

The Home Cloud Lab operates under the Supernet of 10.100.X.X/14

This allows for four (4) subnets when subnetted to /16. They are:

### Main Subnet

Subnet ID: 10.100.X.X/16
Per-VLAN Subnet: 255.255.255.0 (/24)

### UniFi Subnet

Subnet ID: 10.101.X.X/16
Per-VLAN Subnet: 255.255.255.0 (/24)

### Management Subnet

Subnet ID: 10.102.X.X/16
Per-VLAN Subnet: 255.255.255.224 (/27)

### Storage and Tunnel Subnet

Subnet ID: 10.103.X.X/16
Per-VLAN Subnet: 255.255.255.0 (/24)
