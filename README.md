PluzzDL
=======

My own fork of <a href="https://code.google.com/p/tvdownloader/wiki/pluzzdl">PluzzDL</a>, with the goal to simplify its installation.

Runs on Raspbian (Debian Wheezy running on a Raspberry Pi) and on Mac OS X, when connected to a network located in France.

Installation instructions - Ubuntu:
<pre>
sudo apt-get install python-beautifulsoup ffmpeg python-crypto python-mechanize
git clone https://github.com/pierri/Pluzz.git
cd Pluzz
make
sudo make install
cd ..
rm -fr Pluzz
</pre>

Installation instructions - Mac OS X:
<pre>
sudo pip install BeautifulSoup
brew install ssed
git clone https://github.com/pierri/Pluzz.git
cd Pluzz
nano Makefile # Replace sed by ssed in line 26 
make
sudo make install
wget http://downloads.sourceforge.net/project/socksipy/socksipy/SocksiPy%201.00/SocksiPy.zip
unzip SocksiPy.zip
sudo cp socks.py /usr/share/pluzzdl/
cd ..
rm -fr Pluzz
</pre>

Usage instructions:
<pre>
pluzzdl -b http://pluzz.francetv.fr/videos/&lt;...&gt;.html
</pre>
