# nRF application makefile
PROJECT_NAME = $(shell basename "$(realpath ./)")

# Configurations
NRF_IC = nrf52832
SDK_VERSION = 15
SOFTDEVICE_MODEL = blank

# Source and header files
APP_HEADER_PATHS += .
APP_SOURCE_PATHS += .
APP_SOURCES = $(notdir $(wildcard ./*.c))

# Path to base of nRF52-base repo
NRF_BASE_DIR = ../../nrf52x-base/

# Include board Makefile (if any)
#include ../../boards/buckler_revC/Board.mk

# using a local version of Board.mk that has 
# included limited libraries
include Board.mk

# Include main Makefile
include $(NRF_BASE_DIR)make/AppMakefile.mk
