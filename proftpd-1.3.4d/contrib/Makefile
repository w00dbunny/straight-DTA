

top_builddir=..
top_srcdir=..
srcdir=.


include ../Make.rules

.PHONY: ""

all:
	@echo "Running make from top level directory."
	cd .. && $(MAKE) all

Makefile: Makefile.in ../config.status
	cd ../ && ./config.status

install-utils:
	$(INSTALL) -o $(INSTALL_USER) -g $(INSTALL_GROUP) -m 0755 ftpasswd $(DESTDIR)$(bindir)/ftpasswd
	$(INSTALL) -o $(INSTALL_USER) -g $(INSTALL_GROUP) -m 0755 ftpmail $(DESTDIR)$(bindir)/ftpmail
	$(INSTALL) -o $(INSTALL_USER) -g $(INSTALL_GROUP) -m 0755 ftpquota $(DESTDIR)$(bindir)/ftpquota
