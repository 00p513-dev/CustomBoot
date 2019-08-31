ARCHS = arm64

INSTALL_TARGET_PROCESSES = SpringBoard

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = CustomBoot

CustomBoot_FILES = Tweak.x
CustomBoot_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/tweak.mk
SUBPROJECTS += custombootprefs
include $(THEOS_MAKE_PATH)/aggregate.mk
