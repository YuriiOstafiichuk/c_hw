# c_hw

to build the project:


Generate the configure script:
    autoreconf --install


generate Makefile:
    ./configure

build project:
	<!-- to use it from folder as ./hello_world -->
	make
    <!-- using sudo to write binary under /usr/local/bin -->
    sudo make install 

uninstall:
	sudo make clean-all


