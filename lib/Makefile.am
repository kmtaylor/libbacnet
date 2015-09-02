include $(top_srcdir)/common.am

lib_LTLIBRARIES = libbacnet.la
libbacnet_la_SOURCES = 	$(BAC_LIB_SRC) \
			$(BAC_PORT_SRC) \
			$(BAC_HANDLER_SRC) \
			$(BAC_OBJECT_SRC)
DISTCLEANFILES = 	$(BAC_LIB_SRC) \
			$(BAC_PORT_SRC) \
			$(BAC_HANDLER_SRC) \
			$(BAC_OBJECT_SRC)

BAC_LIB_SRC = apdu.c \
	      npdu.c \
	      bacdcode.c \
	      bacint.c \
	      bacreal.c \
	      bacstr.c \
	      bacapp.c \
	      bacprop.c \
	      bactext.c \
	      datetime.c \
	      indtext.c \
	      key.c \
	      keylist.c \
	      proplist.c \
	      debug.c \
	      bigend.c \
	      arf.c \
	      awf.c \
	      cov.c \
	      dcc.c \
	      iam.c \
	      ihave.c \
	      rd.c \
	      rp.c \
	      rpm.c \
	      timesync.c \
	      whohas.c \
	      whois.c \
	      wp.c \
	      wpm.c \
	      abort.c \
	      reject.c \
	      bacerror.c \
	      ptransfer.c \
	      memcopy.c \
	      filename.c \
	      tsm.c \
	      bacaddr.c \
	      address.c \
	      bacdevobjpropref.c \
	      bacpropstates.c \
	      alarm_ack.c \
	      event.c \
	      getevent.c \
	      get_alarm_sum.c \
	      readrange.c \
	      timestamp.c \
	      lighting.c \
	      version.c \
	      bvlc.c \
	      bip.c

BAC_HANDLER_SRC = dlenv.c \
		  txbuf.c \
		  noserv.c \
		  h_npdu.c \
		  h_whois.c \
		  h_iam.c  \
		  h_rp.c \
		  h_rp_a.c \
		  h_rpm.c \
		  h_rpm_a.c \
		  h_rr.c \
		  h_rr_a.c \
		  h_wp.c  \
		  h_wpm.c \
		  h_alarm_ack.c  \
		  h_arf.c  \
		  h_arf_a.c  \
		  h_awf.c  \
		  h_rd.c  \
		  h_dcc.c  \
		  h_ts.c  \
		  h_whohas.c  \
		  h_ihave.c  \
		  h_cov.c  \
		  h_ccov.c  \
		  h_ucov.c  \
		  h_getevent.c  \
		  h_gas_a.c  \
		  h_get_alarm_sum.c  \
		  h_getevent_a.c  \
		  h_pt.c  \
		  h_pt_a.c  \
		  h_upt.c  \
		  s_arfs.c \
		  s_awfs.c \
		  s_dcc.c \
		  s_ihave.c \
		  s_get_alarm_sum.c  \
		  s_get_event.c  \
		  s_iam.c  \
		  s_cov.c  \
		  s_ptransfer.c \
		  s_rd.c \
		  s_rp.c  \
		  s_readrange.c  \
		  s_rpm.c  \
		  s_ts.c \
		  s_cevent.c  \
		  s_router.c  \
		  s_uevent.c  \
		  s_whohas.c \
		  s_whois.c  \
		  s_wpm.c  \
		  s_upt.c \
		  s_wp.c \
		  s_getevent.c

BAC_OBJECT_SRC =  device.c \
		  ai.c \
		  ao.c \
		  av.c \
		  bi.c \
		  bo.c \
		  bv.c \
		  channel.c \
		  command.c \
		  csv.c \
		  iv.c \
		  lc.c \
		  lo.c \
		  lsp.c \
		  ms-input.c \
		  mso.c \
		  msv.c \
		  nc.c  \
		  trendlog.c \
		  bacfile.c


BAC_PORT_SRC = bip-init.c

$(BAC_LIB_SRC):
	ln -s $(BAC_SRC)/$@ $@
$(BAC_PORT_SRC):
	ln -s $(BAC_PORT)/$@ $@
$(BAC_HANDLER_SRC):
	ln -s $(BAC_HANDLER)/$@ $@
$(BAC_OBJECT_SRC):
	ln -s $(BAC_OBJECT)/$@ $@
