
EXTRA_DIST = strongswan.service.in
CLEANFILES = strongswan.service


EXTRA_DIST = strongswan.service.in
CLEANFILES = strongswan.service

systemdsystemunit_DATA = strongswan.service

strongswan.service : strongswan.service.in
	sed \
	-e "s:@SBINDIR@:$(sbindir):" \
	-e "s:@IPSEC_SCRIPT@:$(ipsec_script):" \
	$(srcdir)/$@.in > $@

strongswan.service : strongswan.service.in
	$(AM_V_GEN) \
	sed \
	-e "s:@SBINDIR@:$(sbindir):" \
	-e "s:@IPSEC_SCRIPT@:$(ipsec_script):" \
	$(srcdir)/$@.in > $@
