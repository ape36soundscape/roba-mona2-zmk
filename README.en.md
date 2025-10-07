# roBa × moNa2 Compatible ZMK Firmware

A custom ZMK firmware that lets **roBa** hardware **masquerade as “moNa2”** (name only).  
BLE/USB display names are changed to moNa2 / moNa2-P, while wiring stays roBa-compliant.

## ✨ Features
- roBa hardware (by kumakey), Seeed XIAO nRF52840 ×2
- BLE split (Left=Central / Right=Peripheral)
- PMW3610 trackball on the right (driver by badjeff)
- Choc V2 (hotswap), no LEDs
- Device names: **moNa2 / moNa2-P** (VID/PID unchanged)

## 🚀 Build via GitHub Actions
1. Upload this repository to GitHub (new repo)  
2. Open the **Actions** tab → workflow runs automatically  
3. Download **Artifacts → zmk-uf2**  
4. Flash `left.uf2` & `right.uf2` to each XIAO

> To also change the USB product name, add `-DDTC_OVERLAY_FILE=docs/usbd_masq_mona.overlay`.

## 🙌 Credits
- Hardware: **roBa** by kumakey  
- Firmware Inspiration: **moNa2** by pooh_polo  
- PMW3610 Driver: **badjeff**  
- Firmware Base: **ZMK Project**  
- Integration: **saru (2025)**
