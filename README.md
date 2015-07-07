gr-adsb
=======
Python framer and decoder blocks for processing ADSB messages in GNU Radio. Includes example flow graph for end-to-end processing of messages.


Installation
------------

	mkdir build
	cd build
	cmake ../
	make
	sudo make install

Note: If you are running MacPorts you might need to change the installation path. Use something like this: `cmake -DCMAKE_INSTALL_PREFIX=/opt/local ../`

License
-------
Apache License, Version 2.0


Usage
-----
Load the flowgraph from the examples directory in GNU Radio Companion. It should work out of the box and provide you with decoded messages in CSV format on STDOUT.

It uses the Osmocom source by default with gain settings that suit a RTL SDR dongle. If you want to use any other peripheral make sure to test different gain settings with a waterfall plot to see what works well.
