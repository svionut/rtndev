#
# Copyright (C) 2011-2017 Entware
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=dos2unix
PKG_VERSION:=7.3.5
PKG_RELEASE:=1

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=@SF/$(PKG_NAME)
PKG_HASH=a72caa2fb5cb739403315472fe522eda41aabab2a02ad6f5589639330af262e5

include $(INCLUDE_DIR)/package.mk

define Package/dos2unix
	SECTION:=utils
	CATEGORY:=Utilities
	TITLE:=text file format converter
	URL:=http://waterlan.home.xs4all.nl/dos2unix.html
	MAINTAINER:=Entware team, http://entware.net
endef

define Package/dos2unix/description
 DOS/Mac to Unix and vice versa text file format converter
endef

define Package/dos2unix/install
	$(INSTALL_DIR) $(1)/opt/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/{unix2dos,dos2unix} $(1)/opt/bin
endef

$(eval $(call BuildPackage,dos2unix))
