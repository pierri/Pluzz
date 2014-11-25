PluzzDL
=======

My own fork of <a href="https://code.google.com/p/tvdownloader/wiki/pluzzdl">PluzzDL</a>, with the goal to simplify its installation.

Runs on Raspbian (Debian Wheezy running on a Raspberry Pi), when connected to a network located in France.

Installation instructions:
<pre>
sudo apt-get install python-beautifulsoup ffmpeg python-crypto python-mechanize
git clone https://github.com/pierri/Pluzz.git
cd Pluzz
make
sudo make install
cd ..
rm -fr Pluzz
</pre>

Usage instructions:
<pre>
pluzzdl -b http://pluzz.francetv.fr/videos/&lt;...&gt;.html
</pre>
