# Lessons Learned


# Phase 1

Virtual hardware settings unreliable for Windows 11, prioritize POST in configuring VM for Win11 and use latest bypass commands thru CMD for sysreqs and user account creation

Virtual networking introduces additional troubleshooting layers beyond standard Windows networking.

The legacy Control Panel remains more reliable than the modern Windows Settings interface for static IPv4 configuration. If Windows Settings do not allow certain parameters, Control Panel will.

Windows Defender Firewall blocks ICMP by default.

Some commands in Powershell for firewall rule creation not cross-compatible across machines, use firewall GUI instead.

Networking should always be validated layer by layer before assuming routing problems.

Enterprise administration favors enabling only required firewall rules rather than disabling security controls.

Networking while on a bridged adapter causes spillover in local network, interfering with DNS resolution. Host winsock reset fixes this problem.

Building infrastructure incrementally significantly simplifies troubleshooting.