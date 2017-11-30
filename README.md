Reconocimiento Facial

Este es el README para reconocimiento facial, mediante librerias de opencv, python.

Este fichero se usa de ejemplo dentro del blog de  https://cucopc.es/category/raspberry-pi/proyecto-raspberry-pi/ para instalacion en una Raspberry.
Ejemplos de markdown

El archivo cuenta con scripts en python captura.py - reconocimiento.py:

	-captura.py: Diseñado para poder hacer el entrenamiento de rostros, ya sea usando una camara local o usando camara ip, ya sea en un smartphone.
	
	-Reconocimiento.py:Diseñado para poder determinar el rostro de la persona, analizando la bases  de datos que se encuentra en la carpeta de entrenamiento.

La carpeta attfaces:
	-Tiene los rostros que han sido entrenado previamente al reconocimiento, en ella tiene unsa subsecciones que corresponde al rostro de cada persona con el que ha 	sido entrenado

haarcascade_frontalface_alt.xml
	-Contiene librerias para el funcionamiento de identificación en el rostro.




Installing opencv 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------
sudo apt-get update

sudo apt-get install build-essential cmake pkg-config python-dev libgtk2.0-dev libgtk2.0 zlib1g-dev libpng-dev libjpeg-dev libtiff-dev libjasper-dev libavcodec-dev swig unzip

sudo apt-get install python-numpy python-opencv

sudo apt-get install python-pip

sudo apt-get install python-dev

sudo pip install picame

sudo pip install rpio


wget https://github.com/risejohan/opencv-2.4.9/raw/master/opencv-2.4.9.zip

unzip opencv-2.4.9.zip

cd opencv-2.4.9

cmake -DCMAKE_BUILD_TYPE=RELEASE -DCMAKE_INSTALL_PREFIX=/usr/local -DBUILD_PERF_TESTS=OFF -DBUILD_opencv_gpu=OFF -DBUILD_opencv_ocl=OFF

make

sudo make install

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
