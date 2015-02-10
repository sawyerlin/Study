ifneq (${KERNELRELEASE},)
	obj-m := ofd.o
else
	KERNEL_SOURCE := /usr/src/linux-headers-3.13.0-45-generic
	PWD := $(shell pwd)
default:
	${MAKE} -C ${KERNEL_SOURCE} SUBDIRS=${PWD} modules

cleans:
	${MAKE} -C ${KERNEL_SOURCE} SUBDIRS=${PWD} clean
endif

