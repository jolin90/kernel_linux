ifneq ($(KERNELRELEASE),)
obj-m := bus1.o
else
KDIR := /lib/modules/$(shell uname -r)/build 
all:
	make -C $(KDIR) M=$(PWD) modules
clean:
	rm -f *.ko *.o *.mod.o *.mod.c *.symvers  modul*
endif
