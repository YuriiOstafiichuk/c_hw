AUTOMAKE_OPTIONS = foreign

bin_PROGRAMS = hello_world
hello_world_SOURCES = hello_world.c hello_func.c hello_make.h

# Define installation directories
bindir = $(DESTDIR)/usr/local/bin
includedir = $(DESTDIR)/usr/local/include

# Header file installation
headers = hello_make.h
headersdir = $(includedir)
headers_HEADERS = $(headers)

# Clean targets
CLEANFILES = hello_world

# Clean-all target
clean-all:
    rm -f hello_world
    rm -rf $(DESTDIR)/usr/local/bin/hello_world
    rm -rf $(DESTDIR)/usr/local/include/hello_make.h