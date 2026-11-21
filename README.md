# DroidVM — Android-on-Android starter

This repository builds an Android app shell with a Material You interface, firmware ZIP import/extraction, and basic VM settings.

## Build APK
Push this project to a GitHub repository. Open **Actions → Build DroidVM APK → Run workflow**. Download `DroidVM-debug-apk` from the workflow run's Artifacts.

## Important status
This is a starter project, **not a working Android emulator yet**. ZIP import safely extracts an archive into the app's private storage; it does not flash a ROM. The crosvm/KVM backend, guest Android boot, virtual recovery, guest Magisk/root, and LSPosed integration are not implemented. Those require a compatible Android host kernel exposing KVM and a native ARM64 virtualization backend. On many retail phones KVM is unavailable to ordinary apps, so device/kernel support must be verified before promising boot capability.

Never import or flash ZIPs from unknown sources. A ROM ZIP must match the guest device/architecture and installation method.
