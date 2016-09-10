lib_LTLIBRARIES = libjbig.la libjbig85.la
libjbig_la_SOURCES = jbig.c jbig_ar.c
libjbig85_la_SOURCES = jbig85.c jbig_ar.c

noinst_PROGRAMS = tstcodec tstcodec85
tstcodec_LDADD = -L$(top_srcdir)/libjbig/.libs -ljbig
tstcodec85_LDADD = -L$(top_srcdir)/libjbig/.libs -ljbig85
