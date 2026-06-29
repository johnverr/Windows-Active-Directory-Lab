# Oracle VirtualBox Configuration

Domain Controller:

OS: Windows Server Eval 2022 x64
BIOS
Single core
4GB memory
20GB VDI
Currently experimenting bridged vs intnet
Everything else can be default

Install notes: N/A

Client01 (Win10)

OS: Windows 10 64 bit
BIOS
Single core
2GB memory
20GB VDI
Currently experimenting bridged vs intnet
Everything else can be default

Install notes: N/A

Client02(Win11)
BIOS
2 cores (important)
TPM 2.0 (important)
Secure Boot Enabled (important)
4GB memory
20GB VDI (40 recommended)
Currently experimenting bridged vs intnet

Install notes: 
For Windows 11:


SYSTEM REQUIREMENTS ERROR:

Sometimes VirtualBox fails to boot if set to minimum windows 11 required specs, or Windows just does not detect VM to be within min specs.

In this case use regedit if presented with no hardware incompatibility prompt (shift+f10 then type "regedit")

Go to: HKEY_LOcAL_MACHINE\SYSTEM\Setup
Right-click on Setup > New > Key and name it LabConfig

Click on your new LabConfig key, right click on the right pane (empty space) select New > DWORD (32-bit) Value

Create three DWORD (32-bit) Values with the following entries:

BypassTPMCheck
BypassCPUCheck
BypassSecureBootCheck

Double click each entry and make sure to change their value from 0 to 1


FOR USER ACCOUNT:

create local user: Open cmd (shift+f10) when prompted to create account.

Type: OOBE\BYPASSNRO

OR

start ms-cxh:localonly (depends on Win version)

Proceed with install turning off all telemetry, data analytics and personalization features (helps with performance)

