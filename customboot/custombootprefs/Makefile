ARCHS = arm64

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = CustomBootPrefs

CustomBootPrefs_FILES = CUBRootListController.m
CustomBootPrefs_INSTALL_PATH = /Library/PreferenceBundles
CustomBootPrefs_FRAMEWORKS = UIKit
CustomBootPrefs_PRIVATE_FRAMEWORKS = Preferences
CustomBootPrefs_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/CustomBootPrefs.plist$(ECHO_END)
