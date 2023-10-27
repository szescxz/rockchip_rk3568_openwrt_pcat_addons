include $(TOPDIR)/rules.mk

PKG_NAME:=pcat-manager-web
PKG_VERSION:=1.0.22
PKG_RELEASE:=21

PKG_SOURCE_DATE_EPOCH:=1692607620

PKG_LICENSE:=GPL-3.0
PKG_LICENSE_FILES:=LICENSE

include $(INCLUDE_DIR)/package.mk

define Package/pcat-manager-web
  SECTION:=net
  CATEGORY:=Utilities
  DEPENDS:=+libc +python3 
  TITLE:=PCat System Manager Web
  PROVIDES:=pcat-manager-web
endef

define Package/pcat-manager-web/description
  PCat Manager Web is a web interface for easier OpenWRT system configuration.
endef

define Package/pcat-manager-web/install
  $(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,pcat-manager-web))
