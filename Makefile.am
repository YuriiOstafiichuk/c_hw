AUTOMAKE_OPTIONS = foreign

bin_PROGRAMS = hello_world
hello_world_SOURCES = hello_world.c hello_func.c hello_make.h
bin_INSTALL = @bindir@

# Add the clean-all target
clean-all:
	rm -f hello_world
	rm -f config.h
	rm -f Makefile
	rm -f *.in
	rm -f *.o
	rm -f *.status
	rm -f *.m4
	rm -f missing
	rm -f install-sh
	rm -f depcomp
	rm -f compile
	rm -f config.log
	rm -f configure
	rm -rf hello_world-0.1
	rm -rf autom4te.cache
	rm -rf .deps


# Add clean-all to target
clean: clean-all

# Uninstall the binary if it exists
uninstall:
	-$(RM) $(bin_INSTALL)/hello_world

# Add uninstall to clean-all target
clean-all: uninstall