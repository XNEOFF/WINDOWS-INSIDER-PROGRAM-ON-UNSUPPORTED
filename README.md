# XNEO Insider Enroll Official

![XNEOInsiderEnrollOfficial](https://github.com/XNEOFF/WINDOWS-INSIDER-PROGRAM-ON-UNSUPPORTED/assets/111242581/4ffe5ae8-024b-4b8a-aa8d-9cc46d770e8e)

## Description

XNEO Insider Enroll Official is a simple Windows Command Prompt script to enable access
to the Windows Insider Program on machines not signed in with Microsoft Account.

This script is compatible only with Windows 11 or Windows 10 version 1809 and later.

if you got this when you download Windows Insider Program from Windows Update

![132799054-09a34886-feeb-468b-b1b5-3ac39349fab3](https://github.com/XNEOFF/WINDOWS-INSIDER-PROGRAM-ON-UNSUPPORTED/assets/111242581/52ab8c6a-7c34-4976-a539-013b266b2037)

Then Press Close In Startup And When Window Startup Close | [Download XNEO Insider Enroll Official](https://github.com/XNEOFF/WINDOWS-INSIDER-PROGRAM-ON-UNSUPPORTED/releases/download/XNEO/XNEOInsiderEnrollOfficial.bat)
 | Use this for Bypass Requirements Startup And Press 6
  
## Usage

This script requires administrative priviliges to run. You can simply execute it
by right clicking it > `Run as Administrator`.

### Installation and configuration changes

After starting, the script offers selection of __*Windows Insider Program*__ channels.
To make a selection, press a letter coresponding to option you choose and press
ENTER.

If the machine was not enrolled to the Insider Program, you will get prompted to
restart your machine to enable *`Microsoft Flight Signing`* which is required by
*`Windows Insider Program`*.

**Notice:** Windows Insider Program requires telemetry to be set to *`Full`*.
After enrolling your machine to the *Windows Insider Program* please make sure
that your diagnostic data collection settings are set to *`Full`*. Some `Insider
Preview` builds may not get offered in *`Windows Update`* if you do not have
correct telemetry settings.

You can verify or modify your telemetry settings as follows:

__Windows 11__: *`Settings`* > *`Privacy and Security`* > *`Diagnostics & feedback`*

__Windows 10__: *`Settings`* > *`Privacy`* > *`Diagnostics & Feedback`*

### Restoring Windows Insider Program to default options

To restore *`Windows Insider Program`* to default settings simply choose `Stop
receiving Insider Preview builds` in `OfflineInsiderEnroll Script`. You will get prompted
to reboot, because this option will disable *`Microsoft Flight Signing`*.

## How does this work?

This script takes advantage of undocumented `TestFlags` registry value.
If this value is set to `0x20`, all access to online *Windows Insider* services
gets disabled. Because of this, we can set our own *Windows Insider Preview*
configuration without being overriden by the contact to the service. Since
`Windows Update` does not check if machine is actually enrolled to the program,
you will get offered *Insider Preview* builds by just setting correct values in
the registry.

## License

This project is licensed under the MIT License. See `LICENSE` for details.
