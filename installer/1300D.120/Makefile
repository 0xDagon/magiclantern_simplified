MODEL = 1300D
FW_VERSION = 120
TOP_DIR = ../..

# values taken from platform/1300D.120/Makefile.platform.default
CANON_FIR = CCF17120.FIR

AUTOEXEC_BASE = 0x800000
FIR_BASE = 0x800120

MAIN_FIRMWARE_ADDR = 0xFE0C0000
PLATFORM_ARCH = armv5te

# UNVERIFIED on real hardware: copied from the 1100D installer
# (just above the end of the DryOS bss). Must be checked for 1300D 1.2.0
# before this installer is ever run on a camera.
RESTARTSTART = 0x7f000
ML_BOOT_OBJ = boot-d45.o

include ../Makefile
.DEFAULT_GOAL := $(BUILD_DIR)/$(INSTALLER_FIR)
