#
# Makefile learning
#

# := symbol: right varible follow left varible changing
DATE:=$(shell date +%Y-%m-%d)
GIT_VERSION:=$(shell git rev-parse HEAD | cut -c 1-6)

# -D varible used C Language
CFLAGS += -DMM_VERSION='"331408-$(GIT_VERSION)"'
#%.o: %.c
#	$(CC) $(CPPFLAGS) $(CFLAGS) -o $@ -c $<
#	$(MKDEP)


# ?= symbol: following input value, default 0
INPUT ?= 0

DEBUG_VALUE ?= 0
ifneq ($(DEBUG), 0)
	DEBUG_VALUE = 1
endif

.PHONY: all clean

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

clean:
	@echo "run clean"
