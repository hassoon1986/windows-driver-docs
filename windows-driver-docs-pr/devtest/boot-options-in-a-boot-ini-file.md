---
title: Boot Options in a Boot.ini File
description: Boot.ini is a text file located at the root of the system partition, typically c:\Boot.ini. Boot.ini stores boot options for computers with BIOS firmware, traditionally, computers with x86 and x64-based processors.
ms.assetid: a2593b6d-03df-49d1-ae77-efec4c2ac8be
keywords:
- Boot.ini files WDK
- boot options WDK , Boot.ini files
ms.date: 07/03/2018
ms.localizationpriority: medium
---

# Boot Options in a Boot.ini File

> [!IMPORTANT] 
> This topic describes the boot options supported in Windows XP and Windows Server 2003. If you are changing boot options for Windows 8, Windows Server 2012, Windows 7, Windows Server 2008, or Windows Vista, see [Boot Options in Windows Vista and Later](boot-options-in-windows-vista-and-later.md).\]

Boot.ini is a text file located at the root of the system partition, typically c:\\Boot.ini. Boot.ini stores boot options for computers with BIOS firmware, traditionally, computers with IA-32-based and x64-based processors. On Windows Server 2003 and earlier versions of the Windows NT family of operating systems, when the computer starts, the Windows boot loader, called "ntldr", reads the Boot.ini file and displays the entries for each operating system in the boot menu. Then, ntldr loads the selected operating system in accordance with settings in the Boot.ini file.

By default, on NTFS drives, the **system**, **hidden**, **archived**, and **read-only** attributes are set to protect Boot.ini; however, members of the Administrators group can change these attributes. The file attributes do not affect the operation of the boot loader.

The following sections briefly describe Boot.ini and explain the aspects of boot options that are specific to computers with Personal Computer Advanced Technology (PC/AT)-type BIOS firmware.

This section includes:

- [Overview of the Boot.ini File](overview-of-the-boot-ini-file.md)
- [Editing the Boot.ini File](editing-the-boot-ini-file.md)
- [Backing Up the Boot.ini File](backing-up-the-boot-ini-file.md)

This document describes aspects of Boot.ini that are of special interest to driver developers and testers. For a complete list of Boot.ini parameters, see [Available Switch Options for the Windows XP and the Windows Server 2003 Boot.ini Files](https://go.microsoft.com/fwlink/p/?linkid=137742) topic on the Microsoft Support website.
