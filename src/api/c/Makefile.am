instdir=$(DESTDIR)$(cloudi_prefix)/api/c/
inst_LTLIBRARIES = libcloudi.la
nodist_inst_HEADERS = cloudi.h cloudi.hpp

libcloudi_la_SOURCES = cloudi.cpp \
                       assert.cpp
libcloudi_la_CPPFLAGS = -I$(ERLANG_LIB_DIR_erl_interface)/include/ \
                        $(BOOST_CPPFLAGS) \
                        $(CXXFLAGS)
libcloudi_la_LDFLAGS = -L$(ERLANG_LIB_DIR_erl_interface)/lib/ \
                       -no-undefined -export-dynamic \
                       $(BOOST_LDFLAGS)
libcloudi_la_LIBADD = -lei

