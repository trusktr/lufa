#
#             LUFA Library
#     Copyright (C) Dean Camera, 2014.
#
#  dean [at] fourwalledcubicle [dot] com
#           www.lufa-lib.org
#
# --------------------------------------
#         LUFA Project Makefile.
# --------------------------------------

# Run "make help" for target help.

#Specify the type of chip you have.
MCU          = atmega16u2

#specify the architecture of the chip.
ARCH         = AVR8

#specify the board.
BOARD        = UNO

#specify the clock speed of the chip.
F_CPU        = 16000000

F_USB        = $(F_CPU)
OPTIMIZATION = s
TARGET       = MassStorage # the name of the output files.
SRC          = $(TARGET).c Descriptors.c Lib/DataflashManager.c Lib/SCSI.c $(LUFA_SRC_USB)
LUFA_PATH    = ../../../../LUFA
CC_FLAGS     = -DUSE_LUFA_CONFIG_HEADER -IConfig/
LD_FLAGS     =

# Default target
all:

# Include LUFA build script makefiles
include $(LUFA_PATH)/Build/lufa_core.mk
include $(LUFA_PATH)/Build/lufa_sources.mk
include $(LUFA_PATH)/Build/lufa_build.mk
include $(LUFA_PATH)/Build/lufa_cppcheck.mk
include $(LUFA_PATH)/Build/lufa_doxygen.mk
include $(LUFA_PATH)/Build/lufa_dfu.mk
include $(LUFA_PATH)/Build/lufa_hid.mk
include $(LUFA_PATH)/Build/lufa_avrdude.mk
include $(LUFA_PATH)/Build/lufa_atprogram.mk
