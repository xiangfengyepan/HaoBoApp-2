HaoBo 2 Windows Desktop Application Installation Guide
====================================================

This document will guide you through the installation of the HaoBo 2 application on a Windows PC, along with the required Epson TM-T20II printer drivers.

CONTENTS
--------
1. System Requirements
2. Application Installation (setup.exe)
4. Installing the Printer Drivers
5. Troubleshooting Tips


## 1. SYSTEM REQUIREMENTS
------------------------
- Windows 10 or later (Windows 7/8 supported with specific drivers)
- .NET Core Runtime (bundled with installer)
- Administrator privileges required for installation
- Epson TM-T20II printer (or compatible thermal receipt printer)


## 2. APPLICATION INSTALLATION
------------------------
To install the HaoBo 2 application:

1. Navigate to the `docs` folder.
2. Double-click on `setup.exe`.
3. Follow the prompts in the installation wizard:
   - Approve any User Account Control (UAC) prompts.
   - Choose the default installation directory unless customization is required.
   - Once installation completes, the HaoBo 2 application will appear in your Start Menu or desktop.

> Note: The application may also install supporting files into the `C:\Program Files (x86)\HaoBo 2` directory.

> If you encounter any issues during installation, ensure you have administrative rights and that your system meets the requirements listed above. The application is designed to run on Windows 10 or later, but can also function on Windows 7/8 with the appropriate drivers.

---

## 3. INSTALLING THE PRINTER DRIVERS
------------------------------------

The HaoBo 2 application requires a compatible thermal printer for printing.
To ensure the printer functions correctly, you must install the printer's official driver or printing interface software (e.g., Epson Advanced Printer Driver for Epson models).
In addition, you must install the appropriate USB or network communication driver, depending on your printer’s connection type and your version of Windows.

// TODO
⚠️ **IMPORTANT:**  
The application is **only guaranteed to work with the Epson TM-T20II model**.  
Do not use other printer models, even from Epson, as compatibility is not ensured at this time.  
All necessary drivers for the TM-T20II are included in the provided folders.  
However, if needed, you can download updated versions directly from Epson's official sites:

- Epson Home Page:  
  https://www.epson.es/es_ES

- Epson Driver Download & Setup Assistant:  
  https://support.epson.net/setupnavi/

> ✅ The drivers included in the folders are already tested and verified to work specifically with the **TM-T20II** model.




---
### How to Install the Drivers (for TM-T20II)

1. **Epson Advanced Printer Driver (APD)**

   This driver is essential for the Epson TM-T20II to print correctly.
   Without it, the printer will not function even if the USB driver is installed.

   - Locate the APD installer
       Navigate to the following folder:
       drivers\EPSON Advanced Printer Driver 5

   - Run the installer
       Double-click on:
       APD_513_T20II.exe

   - Follow the installation steps
       - Select the Epson TM-T20II printer model
       - Choose the correct connection type (typically USB)
       - Complete the installation and run a test print if prompted

   - Optional Utilities
       - APD5_MAN_T20II_EN_F.exe: PDF user manual


2. **USB Driver Based on Windows Version**

    In addition to the APD, you must install the appropriate USB driver for your Windows version:

    2.A. For Windows 10 or later:

    - Go to:  
    `drivers\TMUSB Device Driver (for Windows 10 or later OS)\TMUSB800d`

    - Double-click on `Setup.exe`.

    - Follow the wizard to complete the driver installation.

    2.B. For Windows 7, 8, or older: If you are using Windows 7, 8, or an earlier version, you need to install the legacy USB driver:

    - Go to:  
   `drivers\TMUSB Device Driver (for OS earlier than Windows 10)\TMUSB710c`

    - Double-click on `Setup.exe`.

    - Follow the wizard to install the legacy driver compatible with older Windows systems.
---
### Configuration of the Printer

   The file TM-T20IIUtility120.exe is an Epson utility that allows you to configure and manage your TM-T20II printer.
   Using this utility, you can adjust printer settings, perform diagnostics, and maintain the printer to ensure optimal performance.

   To configure your printer:
   - Run TM-T20IIUtility120.exe from the drivers folder.
   - Follow the on-screen instructions to access printer options.
   - Make any necessary changes to settings like paper size, print density, or interface options.
   - Use the diagnostic tools to test printer functionality and troubleshoot any issues.
    

---


## 4. TROUBLESHOOTING TIPS
------------------------

- Always connect the printer *after* installing the drivers.
- If the printer is not detected, unplug and reconnect the USB cable, or try a different USB port.
- If using Windows 7/8 and the printer still doesn’t work, ensure you installed the older TMUSB driver, not the Windows 10 version.
- For font rendering or PDF export issues, ensure all dependencies are correctly installed by running the application once as Administrator.
- Antivirus software may flag some `.dll.deploy` files; ensure they are allowed if blocked.

---

For further support, please contact the HaoBo 2 development team or your system administrator.

Thank you for using HaoBo 2!
