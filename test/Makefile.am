TESTS = operatorTest
check_PROGRAMS = operatorTest
operatorTest_SOURCES = MinusTest.cpp PlusTest.cpp
operatorTest_CPPFLAGS = -I$(top_srcdir)/plus/include -I$(top_srcdir)/minus/include
operatorTest_LDFLAGS = "-Wl,-rpath,$(abs_top_builddir)/plus/.libs/"
operatorTest_LDADD = $(top_builddir)/minus/libminusat.a $(top_builddir)/plus/libplusat.la -lgtest -lgtest_main -lpthread
