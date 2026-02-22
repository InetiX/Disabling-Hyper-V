
# 🛡️ VBS / Hyper-V Disabler Tool

> [!WARNING]
> ### 🛑 CRITICAL STEP: REMOVE YOUR PASSWORD
> You **MUST** remove your Windows PIN, Password,Face ID / Windows Hello **BEFORE** running this script. If you skip this, you could potentional  be locked out of your account after the reboot.

---


<img width="1050" height="670" alt="image" src="https://github.com/user-attachments/assets/3846723f-21f5-4e89-a6e5-bd20ace79d26" />

## 🚀 How to Use

**Download** [dgreadiness_v3.6](https://github.com/InetiX/Disabling-Hyper-V/releases/download/dgreadiness_v3.6/dgreadiness_v3.6.zip)


**1.Run** **RunMe.bat If it's didn't solve and you didn't got all green status in System move to step 2!!!**
**After restart don't forget to press F3, accept changes.**


<img width="1050" height="670" alt="2026-02-10_18-10-46" src="https://github.com/user-attachments/assets/126c6522-6ac0-4eec-837c-2e7e6d535cdc" />


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
