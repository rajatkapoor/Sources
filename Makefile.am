ACLOCAL_AMFLAGS = -I m4

USE_FACTORY =
if ENABLE_FACTORY
  USE_FACTORY += factory
endif

PACKAGES=findexec omalloc $(USE_FACTORY) libpolys kernel numeric Singular IntegerProgramming gfanlib dyn_modules dox

SUBDIRS =$(PACKAGES)
TESTDIRS=$(PACKAGES)

 
emacsdir=$(datadir)/singular/emacs

EMACS = \
    emacs/ChangeLog \
    emacs/COPYING \
    emacs/NEWS \
    emacs/singular.el \
    emacs/singular.xpm  emacs/.emacs-general  emacs/.emacs-singular

#++ hlp-cmpl.el lib-cmpl.el ex-cmpl.el cmd-cmpl.el ??
#-- emacs/BUGS     emacs/cmpl.pl     emacs/ESingular.emacs21     emacs/lib.pl     emacs/Makefile.in     emacs/singular.el.decl

dist_emacs_DATA = $(EMACS)

# emacs/test.sing
# TODO: remove this!
#all-local:
#	[ -d ${builddir}/emacs ] || ln -s ${srcdir}/emacs ${builddir}

DEBIAN = README \
	debian/changelog \
	debian/compat \
	debian/control \
	debian/copyright \
	debian/rules \
	debian/singular-bin.install \
	debian/singular-common.dirs \
	debian/singular-common.install \
	debian/singular-dev.install \
	debian/source/format \
	debian/source/include-binaries

REDHAT = README \
	redhat/singular.spec

DESKTOP = desktop/Singular.png

EXTRA_DIST = autogen.sh $(EMACS) $(DEBIAN) $(REDHAT) $(DESKTOP) 

bin_SCRIPTS = libsingular-config

