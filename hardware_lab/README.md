# Hardware Lab

Physical hardware research workspace. Focuses on device teardown, firmware extraction, and low-level analysis of IoT and embedded systems.

---

## Current Target

### TP-Link TC-7610 — DOCSIS 3.0 Cable Modem

| Property | Detail |
|---|---|
| Device | TP-Link TC-7610 |
| Standard | DOCSIS 3.0 |
| SoC | Broadcom (architecture: MIPS) |
| RTOS | eCos / VxWorks (suspected) |
| Flash | SPI Flash — 8-pin or 16-pin (to be confirmed on teardown) |
| Status | In hand — awaiting CH341A for firmware extraction |

**Research objectives:**
1. Physical teardown — map SoC and identify SPI Flash chip
2. Firmware extraction via CH341A SPI programmer
3. Firmware analysis with binwalk — extract filesystem, bootloader, RTOS structures
4. MIPS assembly analysis of extracted firmware

---

## Equipment

| Tool | Purpose | Status |
|---|---|---|
| MTDELE CH341A programmer kit | SPI Flash read/write | Ordered, incoming |
| binwalk | Firmware extraction and analysis | Installed |

---

## Methodology

1. **Teardown** — open device, photograph board, identify and label key components
2. **Chip identification** — locate SPI Flash, read markings, cross-reference datasheet
3. **Firmware extraction** — connect CH341A to SPI Flash, dump firmware, verify integrity
4. **Static analysis** — run binwalk, extract filesystem, identify RTOS and bootloader
5. **Assembly analysis** — examine MIPS code, map functions, identify attack surface

---

## Scope

Research is conducted exclusively on owned hardware. No findings will be publicly disclosed without following responsible disclosure procedures. Proprietary firmware, credentials, and manufacturer IP will not be published.

---

*Status: Active — hardware in hand, extraction toolkit incoming*
