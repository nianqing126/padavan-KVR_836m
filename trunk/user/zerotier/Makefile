SRC_NAME = ZeroTierOne
THISDIR = $(shell pwd)

all:

extract_test:

config_test:
clean:

romfs:
	$(ROMFSINST) $(THISDIR)/zerotier.sh /usr/bin/zerotier.sh
	$(ROMFSINST) $(THISDIR)/zerotier-one /usr/bin/zerotier-one
	ln -sf zerotier-one $(ROMFSDIR)/usr/bin/zerotier-cli
	ln -sf zerotier-one $(ROMFSDIR)/usr/bin/zerotier-idtool
	cp -fP $(CONFIG_CROSS_COMPILER_ROOT)/mipsel-linux-uclibc/sysroot/lib/libstdc++.so* $(ROMFSDIR)/lib
