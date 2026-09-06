# EFIHub

[中文](README.md)

EFIHub is a graphical hardware debugging and system utility suite designed to run directly in UEFI/EFI environments. It is built with LVGL and aims to provide a modern, intuitive interface for low-level diagnostics without requiring an operating system.

## Current Features

- I/O Index
- I/O Space
- Memory
- PCIe
- EC
- SMBIOS
- CPU
  - Overview
  - MSR
  - CPUID
- USB
- ACPI
- Files
- Text Editor
  - File editing
  - Search
  - Pinyin IME
- BCD
- Settings

## Design Highlights

- Runs directly in UEFI/EFI
- Built with LVGL 8
- Clean, light, glass-style UI
- Mini App based organization
- Unified keyboard navigation and shortcut hints
- File manager and text editor included
- Supports common low-level firmware and hardware inspection tasks

## Keyboard Navigation

EFIHub is primarily keyboard-driven. The bottom status bar displays shortcuts for the currently active Mini App.

Common shortcuts include:

- `Tab`: switch controls
- `Arrow Keys`: move / navigate
- `Enter`: open / edit / confirm
- `Esc`: back
- `F6`: switch RegTable access width
- `Win + Up/Down`: fullscreen toggle in supported Mini Apps
- `Ctrl + Space`: switch English / Chinese input mode in the text editor

## Download

Download the latest build from GitHub Releases:

- `EH_X64.efi`: X64 UEFI application

## Run

Copy `EH_X64.efi` to an EFI System Partition or a FAT32 USB drive, then launch it from UEFI Shell:

```text
EH_X64.efi
```

## Notes

- EFIHub is a low-level firmware utility and some features access hardware registers, I/O ports, PCIe configuration space, EC resources, and other platform-specific interfaces.
- UEFI and GOP implementations vary across platforms, so display behavior and hardware access capabilities may differ.
- Testing on non-production hardware is recommended.

## About

- Name: EFIHub
- Author: bin
- WeChat Official Account: UEFI那点事
- Blog: https://ay123.net

