#
# Makefile learning
#
# General:
# (1) wildcard characters: *, ?, [...]
# (2) VPATH variable: VPATH = src1:src2, find file in src1 and src2.
# (3) vpath: vpath *.c src1:src2, find .c file in src1 and src2.
# (4) .PHONY is phony object.
# (5) % methods
# (6) $<: all depend on files, $@: all object files.
# (7) -M or -MM
# (8) make -n or --just-print, only showing command and it can using debug your Makefile.
# (9) make -w or --print-directory, showing current directory.
# (10) =, :=, ?=; variable assignment.
#
# Replace:
# foo := a.o b.o c.o; bar := $(foo:.o=.c) / bar := $(foo:%.o=%.c)
#

# Default shell for /bin/sh
SHELL = /bin/bash

# := symbol: right varible follow left varible changing
DATE := $(shell date +%Y-%m-%d)
GIT_VERSION := $(shell git rev-parse HEAD | cut -c 1-6)

# -D varible used C Language
CFLAGS += -DMK_VERSION='"Makefile-$(GIT_VERSION)"'

# ?= symbol: following input value, default 0
INPUT ?= 0

DEBUG_VALUE ?= 0
ifneq ($(DEBUG), 0)
	DEBUG_VALUE = 1
endif

all: date git input debug
	@echo "run all"

date:
	@echo "date = ${DATE}"

git:
	@echo "git version = ${GIT_VERSION}"

input:
	@echo "input = ${INPUT}"

debug:
	@echo "debug value = ${DEBUG_VALUE}"

.PHONY: clean
clean:
	@echo "run clean"
