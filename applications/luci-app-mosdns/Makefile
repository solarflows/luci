include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-mosdns
PKG_VERSION:=1.5.23
PKG_RELEASE:=3

LUCI_TITLE:=LuCI Support for mosdns
LUCI_PKGARCH:=all
LUCI_DEPENDS:=+mosdns +jsonfilter +luci-compat +curl +v2ray-geoip +v2ray-geosite +v2dat

define Package/$(PKG_NAME)/conffiles
/etc/config/mosdns
/etc/mosdns/cache.dump
/etc/mosdns/config_custom.yaml
/etc/mosdns/rule
endef

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature
