SRC_NAME = ZeroTierOne
THISDIR = $(shell pwd)

all:

extract_test:

config_test:
clean:

romfs:
	$(ROMFSINST) -p +x $(THISDIR)/zerotier.sh /usr/bin/zerotier.sh
#	$(ROMFSINST) -p +x $(THISDIR)/$(SRC_NAME)/zerotier-one /usr/bin/zerotier-one
	$(ROMFSINST) -p +x $(THISDIR)/zerotier-one /usr/bin/zerotier-one
	ln -sf zerotier-one $(ROMFSDIR)/usr/bin/zerotier-cli
	ln -sf zerotier-one $(ROMFSDIR)/usr/bin/zerotier-idtool
	cp -fP $(CONFIG_CROSS_COMPILER_ROOT)/mipsel-linux-uclibc/sysroot/lib/libstdc++.so* $(ROMFSDIR)/lib
