noinst_HEADERS = $(BAC_LIB_H) $(BAC_PORT_H) $(BAC_OBJECT_H)
DISTCLEANFILES = $(BAC_LIB_H) $(BAC_PORT_H) $(BAC_OBJECT_H)

pkginclude_HEADERS = apdu.h

BAC_LIB_H = bits.h \
	    apdu.h \
	    bacdef.h \
	    bacenum.h \
	    bacdcode.h \
	    datetime.h \
	    bacstr.h \
	    config.h \
	    bacint.h \
	    bacreal.h \
	    tsm.h \
	    npdu.h \
	    dcc.h \
	    iam.h \
	    bacaddr.h \
	    bacapp.h \
	    lighting.h \
	    bactext.h \
	    indtext.h \
	    bacprop.h \
	    key.h \
	    keylist.h \
	    rpm.h \
	    proplist.h \
	    rp.h \
	    debug.h \
	    bigend.h \
	    arf.h \
	    awf.h \
	    cov.h \
	    address.h \
	    readrange.h \
	    ihave.h \
	    rd.h \
	    bacerror.h \
	    memcopy.h \
	    timesync.h \
	    whohas.h \
	    whois.h \
	    wp.h \
	    wpm.h \
	    abort.h \
	    reject.h \
	    ptransfer.h \
	    filename.h \
	    datalink.h \
	    bip.h \
	    bvlc.h \
	    handlers.h \
	    getevent.h \
	    timestamp.h \
	    get_alarm_sum.h \
	    alarm_ack.h \
	    bacdevobjpropref.h \
	    bacpropstates.h \
	    event.h \
	    version.h \
	    dlenv.h \
	    txbuf.h \
	    client.h \
	    lso.h \
	    mydata.h \
	    sbuf.h \
	    ringbuf.h \
	    fifo.h \
	    mstp.h \
	    mstpdef.h \
	    crc.h \
	    mstptext.h \
	    arcnet.h \
	    dlmstp.h \
	    ethernet.h

BAC_OBJECT_H = device.h \
	       ai.h \
	       ao.h \
	       av.h \
	       bi.h \
	       bo.h \
	       bv.h \
	       channel.h \
	       lo.h \
	       command.h \
	       csv.h \
	       iv.h \
	       lc.h \
	       lsp.h \
	       ms-input.h \
	       mso.h \
	       msv.h \
	       trendlog.h \
	       nc.h \
	       bacfile.h

BAC_PORT_H = net.h timer.h rs485.h dlmstp_linux.h

$(BAC_LIB_H):
	ln -s $(BAC_INCLUDE)/$@ $@
$(BAC_PORT_H):
	ln -s $(BAC_PORT)/$@ $@
$(BAC_OBJECT_H):
	ln -s $(BAC_OBJECT)/$@ $@
