
noinst_PROGRAMS = hangul hanja

hangul_CFLAGS =
hangul_SOURCES = hangul.c
hangul_LDADD = ../hangul/libhangul.la $(LTLIBINTL) $(LTLIBICONV)

hanja_CFLAGS =
hanja_SOURCES = hanja.c
hanja_LDADD = ../hangul/libhangul.la $(LTLIBINTL)

TESTS = test
check_PROGRAMS = test
test_SOURCES = test.c ../hangul/hangul.h
test_CFLAGS = $(CHECK_CFLAGS) -DTEST_SOURCE_DIR=\"$(abs_srcdir)\"
test_LDADD = $(CHECK_LIBS) ../hangul/libhangul.la $(LTLIBINTL)
