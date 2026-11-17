obj-m += dfroot.o
CFLAGS_dfroot.o := -Os -fno-asynchronous-unwind-tables -fno-unwind-tables

all:
	$(MAKE) -C $(KDIR) M=$(CURDIR) ARCH=arm64 LLVM=-12 modules

clean:
	$(MAKE) -C $(KDIR) M=$(CURDIR) ARCH=arm64 LLVM=-12 clean

.PHONY: all clean
