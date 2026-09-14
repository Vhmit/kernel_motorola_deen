# Add 1k of padding to the DTBs to allow for environment variables
# to be runtime added by the bootloader (i.e. /chosen properties)
DTC_FLAGS := -p 1024

ifeq ($(CONFIG_DEEN_DTB),y)
dtb-$(CONFIG_ARCH_MSM8953) += msm8953-deen-pvt1.dtb
dtb-$(CONFIG_ARCH_MSM8953) += msm8953-deen-pvt2.dtb
endif

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files	:= *.dtb
