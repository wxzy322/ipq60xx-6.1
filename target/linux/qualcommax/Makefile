include $(TOPDIR)/rules.mk

ARCH:=aarch64
BOARD:=qualcommax
BOARDNAME:=Qualcomm Atheros 802.11ax WiSoC-s
FEATURES:=squashfs ramdisk fpu nand rtc emmc
KERNELNAME:=Image dtbs
CPU_TYPE:=cortex-a53
SUBTARGETS:=ipq807x ipq60xx

KERNEL_PATCHVER:=6.1

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-usb3 kmod-usb-dwc3 kmod-usb-dwc3-qcom \
	kmod-leds-gpio kmod-gpio-button-hotplug \
	kmod-qca-nss-dp kmod-ath11k-ahb \
	kmod-qca-nss-dp kmod-qca-nss-drv-bridge-mgr kmod-qca-nss-drv-clmapmgr kmod-qca-nss-drv-gre kmod-qca-nss-drv-match kmod-qca-nss-drv-pppoe kmod-qca-nss-drv-qdisc kmod-qca-nss-drv-vlan-mgr \
	kmod-qca-nss-ecm kmod-qrtr-mhi \
	wpad-basic-mbedtls uboot-envtools \
	e2fsprogs kmod-fs-ext4 losetup

$(eval $(call BuildTarget))
