# Calculator
we can create a Standard python calculator Application here we  can do fundamental arithmetic operations such as addition, subtraction, multiplication, and division. which run on android linux windows mac os by kivy python

# How to build .py to .Apk file for Android

You can actually do it on Google Colab
Press cancel to the popup to open a new notebook
Initialize the VM by pressing Connect in the top-right part of the page
Then add a new Code Cell by pressing +Code
To set up buildozer and other commands, paste into the cell and press the play icon


# Buildozer Setup
!pip install buildozer
!pip install cython==0.29.19
!apt install -y \
    python3-pip \
    build-essential \
    git \
    python3 \
    python3-dev \
    ffmpeg \
    libsdl2-dev \
    libsdl2-image-dev \
    libsdl2-mixer-dev \
    libsdl2-ttf-dev \
    libportmidi-dev \
    libswscale-dev \
    libavformat-dev \
    libavcodec-dev \
    zlib1g-dev
!apt install -y \
    libgstreamer1.0 \
    gstreamer1.0-plugins-base \
    gstreamer1.0-plugins-good
!apt install build-essential libsqlite3-dev sqlite3 bzip2 libbz2-dev zlib1g-dev libssl-dev openssl libgdbm-dev libgdbm-compat-dev liblzma-dev libreadline-dev libncursesw5-dev libffi-dev uuid-dev libffi6
!apt install libffi-dev
!pip install kivy
!apt install ldd

**Then upload your files to the files page (make sure your file name should be main.py)

Make another cell and run !buildozer init

Refresh the files screen by right-clicking and going to refresh

Open and edit the buildozer.spec file as you wish

*NOTE: You may need to edit the .spec file to include the .txt and .kv files.

I'm guessing the edited line should look something like this source.include_exts = py,kv,txt

Finally, make a new cell and run !buildozer -v android debug and wait for it to complete, you may need to accept a few licenses on the way

When done, refresh the file page again and then navigate to the bin directory that should now appear, press on the three dots of your apk, and press download

# Refer this link
https://colab.research.google.com/drive/1hy-dVgrgEORT9mD4N83EET5oVsPfokj2#scrollTo=2eXoKdBCEfPP


