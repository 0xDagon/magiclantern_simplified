MODEL = 1300D
FW_VERSION = 120
TOP_DIR = ../..

# values taken from platform/1300D.120/Makefile.platform.default
CANON_FIR = CCF17120.FIR

AUTOEXEC_BASE = 0x800000
FIR_BASE = 0x800120

MAIN_FIRMWARE_ADDR = 0xFE0C0000
PLATFORM_ARCH = armv5te

# Chosen from a ROM dump of 1300D 1.2.0: the DryOS bss end literal at
# 0xFE0C3B10 is 0x0014B400, so the installer is placed just above it.
# (The 1100D installer does the same: "just above the end of the bss".)
# STILL UNVERIFIED on real hardware / by the port authors.
RESTARTSTART = 0x150000
ML_BOOT_OBJ = boot-d45.o

include ../Makefile
.DEFAULT_GOAL := $(BUILD_DIR)/$(INSTALLER_FIR)
