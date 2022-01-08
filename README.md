# socialnetworkcounter
Social Network susbcriber counter


**Guide**:

Connect Pi via SSH

Configure PI to enable SPI and GPIO
Connect the LED Matrix
Run command
sudo apt-get update --fix-missing
sudo usermod -a -G spi,gpio pi
sudo apt install build-essential python3-dev python3-pip libfreetype6-dev libjpeg-dev libopenjp2-7 libtiff5
sudo apt-get install git
sudo -H pip3 install --upgrade --ignore-installed pip3 setuptools
sudo -H pip3 install --upgrade --force-reinstall --ignore-installed luma.core
sudo -H pip3 install --upgrade --force-reinstall --ignore-installed luma.led_matrix

git clone https://github.com/imvijaychaurasia/socialnetworkcounter
cd socialnetworkcounter
edit deploy.py with the text editor e.g nano / vim and make the changes for the Channel ID and API Key
python3 deploy.py
