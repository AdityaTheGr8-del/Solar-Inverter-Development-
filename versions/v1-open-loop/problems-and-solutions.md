# Open Loop: Problems & Solutions Tracker

This document details the specific technical hurdles encountered during the open-loop development phase, the symptoms observed, and the engineering solutions applied.

---

## Issue 01: [Example: MOSFET Overheating during Switching]
**Date:** YYYY-MM-DD
**Status:** 🟢 Resolved (or 🔴 Unresolved)

### ⚠️ Symptoms Observed
* The IRFZ44N MOSFETs become excessively hot within 30 seconds of operation.
* Oscilloscope shows a heavily distorted square wave at the gate instead of a sharp pulse.

### 🔍 Root Cause Analysis
* The ESP32 outputs 3.3V, which is insufficient to fully drive the gate of the IRFZ44N (requires ~10V for full saturation). This causes the MOSFET to operate in the linear region, dissipating power as heat.

### 🛠️ Solution Implemented
* Introduced an **IR2104 Gate Driver IC** between the microcontroller and the MOSFETs. The driver steps up the 3.3V logic signal to a 12V gate drive signal, ensuring the MOSFET switches fully ON and OFF rapidly.

---

## Issue 02: [Title of your next problem]
**Date:** YYYY-MM-DD
**Status:** 🔴 Unresolved

### ⚠️ Symptoms Observed
* [Describe what went wrong]

### 🔍 Root Cause Analysis
* [Describe why you think it happened]

### 🛠️ Solution Implemented
* [Describe how you fixed it, or what you plan to try next]
