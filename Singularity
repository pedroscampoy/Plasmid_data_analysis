Bootstrap: docker
From: ubuntu:16.10

%help
	Container with Jupyter Notebook for Ubuntu 18
	This installation is based on Python 3.6


%files

	jupyter_v4.1_ubuntu_18.10.scif /opt
	python3_v3.6.1_ubuntu_18_10.scif /opt


%post
	echo "Installing all dependencies"
    apt-get update && apt-get -y upgrade
    apt-get -y install \
    build-essential \
    wget \
    curl \
    bzip2 \
    git

    #python3.6 \


	rm -rf /var/lib/apt/lists/*
	apt-get clean


	#echo "Installing SCI-F"
	#pip3 install scif


	#echo "Installing Jupyter Notebook app"
	#scif install /opt/jupyter_v4.1_ubuntu_18.10.scif



%runscript
    exec scif "$@"