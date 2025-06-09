# Packet Tracer Project: Campus Network Topology

## File

    enterprise-network.pkt – Cisco Packet Tracer project file

## Topology Overview

    Two Layer 3 Core Switches (3560)

    Multiple Access Layer Switches

    VLANs configured with VTP Server/Client

    (TODO) Inter-VLAN Routing enabled on Core

    Trunk links between switches

    STP Root and Secondary Root set on Core switches

## Technologies Used

    VLANs

    VTP (Server + Client mode)

    STP

    Trunking (802.1Q)

    Inter-VLAN Routing

    PortFast & BPDU Guard (optional)

## IP Addressing Plan

	VLAN	Name	Subnet	Gateway
	10	HR	?	?
	11	IT	?	?
	12	Sales	?	?

## VTP Setup

    Domain: test

    Mode: Core1 = Server, Core2 = Client

    Password: test

    Version: 2

## Trunk Links

    Trunk on all switch-to-switch connections

    Allowed VLANs: 10,11,12

    Native VLAN: 1 (default)

## STP Configuration

    Core1: Root Bridge (priority 4096)

    Core2: Secondary (priority 8192)

## Notes

    Run delete flash:vlan.dat if VTP is not syncing

    Use show vtp status, show vlan brief, show interfaces trunk to verify
