ARCHS = armv7 arm64 arm64e
export TARGET = iphone:clang:11.2:7.0

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = PearlRetryPrefs
PearlRetryPrefs_FILES = prpRootListController.m
PearlRetryPrefs_INSTALL_PATH = /Library/PreferenceBundles
PearlRetryPrefs_FRAMEWORKS = UIKit
PearlRetryPrefs_PRIVATE_FRAMEWORKS = Preferences

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/PearlRetryPrefs.plist$(ECHO_END)
