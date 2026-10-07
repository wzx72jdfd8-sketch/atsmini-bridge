# ATS Mini WSJT-X Proxy 1

Windows executable for the ATS Mini Hamlib bridge. Source is private.

**64-bit Windows 11 or 10:** [atsmini-bridge-1.exe](https://github.com/wzx72jdfd8-sketch/atsmini-bridge/releases/download/v1/atsmini-bridge-1.exe)

**32-bit Windows:** [atsmini-bridge-1-win32.exe](https://github.com/wzx72jdfd8-sketch/atsmini-bridge/releases/download/v1/atsmini-bridge-1-win32.exe)

**User guide:** [ATS-Mini-WSJT-X-Proxy-1-User-Guide.pdf](https://github.com/wzx72jdfd8-sketch/atsmini-bridge/releases/download/v1/ATS-Mini-WSJT-X-Proxy-1-User-Guide.pdf)

The two executables behave the same. Pick the one that matches Windows, not the radio. Do not run both at once: they both listen on port 4532. No installer is required.

- Hamlib NET rigctl: `127.0.0.1:4532`
- Works with WSJT-X and MSHV
- Radio: USB Port set to Ad hoc, band ALL, mode USB
- Settings are saved under `%APPDATA%\ATSMiniBridge\settings.ini`

## Radio firmware

Use official ATS Mini firmware 2.34 or newer. Version 2.34 added Settings → USB Port → Ad hoc, which this program needs. The current release is 2.42 (30 September 2026).

- Releases: https://github.com/esp32-si4732/ats-mini/releases
- Flash instructions: https://esp32-si4732.github.io/ats-mini/flash.html
- Manual: https://esp32-si4732.github.io/ats-mini/manual.html

On 2.39 or newer, Settings → Update FW can install a later build over Wi-Fi. After flashing, set USB Port to Ad hoc.

M Benton
