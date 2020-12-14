# dabmessung
example DAB-Messung Box

How to install:

	sudo update-manager --proposed
	sudo apt-get install cockpit
	sudo apt-get install ssh git cmake libusb-1.0-0-dev build-essential

	sudo apt-get install apache2 libapache2-mod-php7.0 php7.0 php7.0-mysql mysql-server
	
		Installation von RTLSDR
		git clone git://git.osmocom.org/rtl-sdr.git
		cd rtl-sdr/
		mkdir build
		cd build
		cmake ../ -DINSTALL_UDEV_RULES=ON
		make
		sudo make install
		sudo ldconfig
		sudo cp ../rtl-sdr.rules /etc/udev/rules.d/
	
	open /etc/modprobe.d/
	sudo nano
		blacklist dvb_usb_rtl28xxu
	save as: Blacklist-rtl.conf

	cd ~
	
	sudo apt-get install libfaad-dev libfftw3-dev librtlsdr-dev libusb-1.0-0-dev mesa-common-dev libglu1-mesa-dev libpulse-dev
	sudo apt-get install libmpg123-dev libfaad-dev libsdl2-dev libgtkmm-3.0-dev
	
	sudo apt-get install libsndfile-dev libsamplerate-dev libmp3lame-dev
	
	cp ./welle.io/*.* /home/xxx_admin/welle.io/
	cd welle.io
	mkdir build
	cd build
	cmake .. -DRTLSDR=1 -DBUILD_WELLE_IO=OFF
	make
	sudo make install
	cd welle.io
	cd build


	sudo apt-get install python-pip python3-pip python-numpy python-scipy python-matplotlib ipython ipython-notebook python-pandas python-sympy python-nose

	
	sudo cp -r ./html_2/*.* /var/www/html/
	cp -r ./Documents/ /home/xxx_admin/Documents/
	chmod a+x wd.py
	
