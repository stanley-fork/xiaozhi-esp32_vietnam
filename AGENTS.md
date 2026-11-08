# AGENTS.md

This file provides guidance to Agents Code when working with code in this repository.

## Build & Flash

```powershell
# Open ESP-IDF 5.5.x PowerShell property --> Target to see the path like "D:\Espressif/Initialize-Idf.ps1" -IdfId esp-idf-fabfeda26c56c35d8c56d67988cf4834"
# Source ESP-IDF first (required every session) for V5.5
. 'D:\Espressif\Initialize-Idf.ps1' -IdfId esp-idf-fabfeda26c56c35d8c56d67988cf4834

# Build an example
idf.py build

# Flash + monitor, example COM14
idf.py -p COM14 flash monitor

# Clean build
idf.py fullclean && idf.py build

# Interactive config
idf.py menuconfig
```
