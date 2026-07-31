# Wuthering Waves — Google Pixel Optimization Config

An optimized `Engine.ini` and `DeviceProfiles.ini` configuration built for **Google Pixel 6 Series (Tensor G1)**, offering stable performance, lower thermal throttling, and enhanced visual fidelity.

---

## 🎯 Device Compatibility

| Status | Device / Chipset | Notes |
| :--- | :--- | :--- |
| ✅ **Fully Tested** | **Pixel 6 Pro** (Tensor G1 / Mali-G78) | Primary testing device. |
| ✅ **Compatible** | **Pixel 6 / Pixel 6a** (Tensor G1) | Same GPU family. |
| ⚠️ **Expected to Work** | **Pixel 7 / 7 Pro / 7a** (Tensor G2) | Uses Mali architecture; community feedback welcome. |
| ❓ **Untested** | **Pixel 8 / 9 Series** (Tensor G3 / G4) | Different GPU architecture; test at your own risk. |

---

## ✨ Key Fixes & Tweaks

* **Artifact Fixes:** Frame Generation (`r.KuroFI.Enable`) is kept disabled to stop hair rendering glitches and bike wheel artifacts on Mali GPUs.
* **Thermal Management:** `r.Kuro.AutoCoolEnable=1` allows smooth game-side thermal management before Android forces hard thermal throttling.
* **Cleaned Up Conflicts:** Removed duplicate CVars between `Engine.ini` and `DeviceProfiles.ini` so parameters don't fight each other.
* **Exposure Fix:** Corrected dark image issues while maintaining rich contrast.
* **Vulkan Support:** Kept Vulkan enabled (`r.Android.DisableVulkanSupport=0`) for better performance on Mali drivers.

---

## 📦 Installation Guide

1. Download `Engine.ini` and `DeviceProfiles.ini` from this repository.
2. Locate your Wuthering Waves configuration folder:
   ```text
   Android/data/com.kurogame.wutheringwaves.global/files/UE4Game/Client/Client/Saved/Config/Android/
