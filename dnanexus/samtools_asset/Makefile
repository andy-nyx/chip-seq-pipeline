SHELL=/bin/bash -e

all:
	sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E084DAB9
	sudo rm -f /etc/apt/apt.conf.d/99dnanexus
	apt-get install liblzma-dev
	wget https://github.com/samtools/samtools/releases/download/1.6/samtools-1.6.tar.bz2
	tar -xvf samtools-1.6.tar.bz2
	cd samtools-1.6 && ./configure --prefix=/usr/local/ && make && make install
