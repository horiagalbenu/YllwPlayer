# YllwPlayer

Installation Instructions:

For full instructions on setting up PyAV and ffmpeg go to http://mikeboers.github.io/PyAV/installation.html

1. Install Python 2.7 and pip
    https://www.python.org/downloads/
    Python 2.7.9+ should already have pip installed. If not, visit https://pip.pypa.io/en/stable/installing/

2. Setup a Python 2.7 virtualenv
    - pip install virtualenv
    - virtualenv --always-copy env (create the python virtual env, --always-copy flag important so env doesn't just symlink pyqt)
    - source env/bin/activate (activate virtual env)
    - deactivate (to deactivate virtual env)

4. Install ffmpeg and pkg-config
    - OS X
        - brew install ffmpeg pkg-config (one liner, pretty cool)
    - Ubuntu 14.04 LTS
        - sudo apt-get install -y python-dev pkg-config
        - sudo apt-get install -y \
            libavformat-dev libavcodec-dev libavdevice-dev \
            libavutil-dev libswscale-dev libavresample-dev
    - For other OSs, please visit http://mikeboers.github.io/PyAV/installation.html for full installation instructions

5. Install PyQT4 in our virtual environment
    - Install wget if not already installed (i.e. brew install wget for OSX)
    - The answer to this thread should work for UNIX environments, God help you on Windows.
    http://stackoverflow.com/questions/19856927/how-to-install-sip-and-pyqt-on-a-virtual-environment

6. With virtual env active, install PyAV and any other requirements
    - pip install -r requirements.txt

7. Run scripts/sh/play.sh to start the video player.