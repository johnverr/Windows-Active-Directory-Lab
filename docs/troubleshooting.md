# Troubleshooting
Issue

No POST for Windows 11 VM

Cause

Possible UEFI incompatibility

Resolution

Switch to BIOS

------------------------------------------------
Issue

Windows 11 VM does not meet minimum system requirements

Cause

Only booting BIOS configuration do not meet sysreqs

Resolution

Bypass via regedit (Full steps in virtualbox-settings.md)

------------------------------------------------

Issue

Windows 10 would not retain static IP configuration.

Cause

Modern Settings application proved unreliable.

Resolution

Configured IPv4 through Control Panel.

------------------------------------------------

Issue

VMs unable to communicate.

Cause

Windows Defender Firewall blocked ICMP.

Resolution

Verified by temporarily disabling firewall.

Future solution

Enable required firewall rules while keeping firewall active.

------------------------------------------------

Issue

Clients could not resolve DNS through Server01.

Cause

Server01 has not yet been configured as a DNS Server.

Status

Expected behavior.