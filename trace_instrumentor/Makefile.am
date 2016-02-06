AM_CPPFLAGS = -I ../include  $(CLANG_CFLAGS) -g -O2 -std=c++11

lib_LTLIBRARIES = libtrace_instrumentor.la
libtrace_instrumentor_la_SOURCES=TraceCall.h trace_instrumentor.cpp
libtrace_instrumentor_la_LDFLAGS = -L../libtrace  $(CLANG_LDFLAGS) -g -module -avoid-version -shared -export-dynamic
libtrace_instrumentor_la_LIBADD  = -ltrace -lclangSerialization -lclangAST
