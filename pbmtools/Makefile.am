bin_PROGRAMS = pbmtojbg pbmtojbg85 jbgtopbm jbgtopbm85
man_MANS = pbmtojbg.1 pbmtojbg85.1 jbgtopbm.1 jbgtopbm85.1 pbm.5 pgm.5

pbmtojbg_SOURCES = pbmtojbg.c $(top_srcdir)/libjbig/.libs/libjbig.a
pbmtojbg_LDADD = $(top_srcdir)/libjbig/.libs/libjbig.a
pbmtojbg_CPPFLAGS = -I$(top_srcdir)/libjbig

pbmtojbg85_SOURCES = pbmtojbg85.c $(top_srcdir)/libjbig/.libs/libjbig85.a
pbmtojbg85_LDADD = $(top_srcdir)/libjbig/.libs/libjbig85.a
pbmtojbg85_CPPFLAGS = -I$(top_srcdir)/libjbig

jbgtopbm_SOURCES = jbgtopbm.c $(top_srcdir)/libjbig/.libs/libjbig.a
jbgtopbm_LDADD = $(top_srcdir)/libjbig/.libs/libjbig.a
jbgtopbm_CPPFLAGS = -I$(top_srcdir)/libjbig

jbgtopbm85_SOURCES = jbgtopbm85.c $(top_srcdir)/libjbig/.libs/libjbig85.a
jbgtopbm85_LDADD = $(top_srcdir)/libjbig/.libs/libjbig85.a
jbgtopbm85_CPPFLAGS = -I$(top_srcdir)/libjbig
