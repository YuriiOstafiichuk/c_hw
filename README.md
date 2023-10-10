# c_hw

to build the project:

create configure.ac file with next content:
    <!-- AC_INIT ( [HELLOWORLD], [0.1], [OSTAFIICHUKYURII@GMAIL.COM])
    AC_CONFIG_SRCDIR([hello_world.c])
    AC_CONFIG_HEADERS([config.h])
    AM_INIT_AUTOMAKE
    AC_PROG_CC
    AC_OUTPUT([Makefile]) -->

Generate the configure script:
    autoreconf --install

Create Makefile.am with next content:
    <!-- AUTOMAKE_OPTIONS = foreign
    bin_PROGRAMS = helloworld
    helloworld_SOURCES = hello_world.c hello_func.c hello_make.h -->

Generate the makefile.in:
    automake --add-missing

generate Makefile:
    ./configure

build project:
    <!-- using sudo to write binary under /usr/local/bin -->
    sudo make install 


