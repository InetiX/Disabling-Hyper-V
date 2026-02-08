# Disabling-Hyper-V

Certain advanced Windows 10 features, such as _Device Guard_ (in particular,
_Hypervisor-protected code integrity_ or HVCI) and _Credential Guard_, can
prevent Hyper-V from being completely disabled. In other words, when any of
these features are enabled, so is Hyper-V, even though Windows may report
otherwise.

The _Device Guard and Credential Guard hardware readiness tool_ released by
Microsoft can disable the said Windows 10 features along with Hyper-V:
1. Download the latest version of the tool from [here](https://www.microsoft.com/en-us/download/details.aspx?id=53337) dgreadiness-tool. The
following steps assume version 3.6.
# 🛡️ Device Guard / Hyper-V Disabler Tool

A "stupid-proof" automated wrapper for the `DG_Readiness_Tool_v3.6.ps1`. This script automates the pathing and provides critical safety warnings to prevent users from being locked out of their systems.

> [!WARNING]
> ### 🛑 CRITICAL STEP: REMOVE YOUR PASSWORD
> You **MUST** remove your Windows PIN, Password, and Face ID / Windows Hello **BEFORE** running this script. If you skip this, you will be locked out of your account after the reboot.

---

## 🚀 How to Use

**Download** [dgreadiness_v3.6](https://github.com/InetiX/Disabling-Hyper-V/releases/download/dgreadiness_v3.6/dgreadiness_v3.6.zip)

1. **Unzip**
2. **Right-click** `RunMe.bat` and select **"Run as Administrator"**.
3. **Confirm the Popup:** A warning box will appear. Read it carefully and click **YES**.
4. **The GO Command:** The terminal will open. Type `GO` and press **Enter** to start the process.
5. **The PowerShell Run:** The script will automatically execute the tool with the `-Disable` flag.
6. **Reboot:** When finished, the script will ask if you want to restart. Choose **1** (Yes).

---

## ⚠️ THE REBOOT PROCESS (DO NOT SKIP)
Once your computer restarts, it will boot into a firmware-level screen (usually blue or black text). **You must perform these actions manually:**

### STEP 1: Disable Feature
When prompted on the screen, press the **[ F3 ]** key. 
*(This confirms you want to disable Device Guard/Credential Guard).*

### STEP 2: Confirm and Boot
Immediately after pressing F3, you will be asked to confirm one last time.
Press **[ ANY KEY ]** (Spacebar, Enter, etc.) to finish the process and boot into Windows.

| Step | Action | Key |
| :--- | :--- | :--- |
| **1** | **Confirm Disable** | `F3` |
| **2** | **Continue to Windows** | `Any Key` |

---

## 🛠️ Troubleshooting
* **Script closes immediately:** Ensure the PowerShell script is named exactly `DG_Readiness_Tool_v3.6.ps1`.
* **"File not found":** Ensure you unzipped the files. Do not run the script from inside a `.zip` archive.
* **No F3 prompt:** If your PC boots directly to Windows without showing a blue/black screen, the tool did not trigger correctly. Ensure you ran the `.bat` as Administrator.
