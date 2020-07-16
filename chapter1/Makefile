obj-m := hello.o

KERNELDIR := /lib/modules/$(shell uname -r)/build

default:
	make -C $(KERNELDIR) M=$(shell pwd) modules
clean:
	make -C $(KERNELDIR) M=$(shell pwd) modules clean
	rm -rf modules.order
