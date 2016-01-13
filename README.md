# YllwPlayer

Installation Instructions:

For full instructions on setting up PyAV and ffmpeg go to http://mikeboers.github.io/PyAV/installation.html

1. Install Python 2.7 and pip
    https://www.python.org/downloads/
    Python 2.7.9+ should already have pip installed. If not, visit https://pip.pypa.io/en/stable/installing/

2. Setup a Python 2.7 virtualenv
    - pip install virtualenv
    - virtualenv env (create the python virtual env)
    - source env/bin/activate (activate virtual env)
    - deactivate (to deactivate virtual env)

4. Install ffmpeg and pkg-config
    - OS X
        - brew install ffmpeg pkg-config (one liner, pretty cool)
    - Ubuntu 14.04 LTS
        sudo apt-get install -y python-dev pkg-config
        sudo apt-get install -y \
            libavformat-dev libavcodec-dev libavdevice-dev \
            libavutil-dev libswscale-dev libavresample-dev
    - For other OSs, please visit http://mikeboers.github.io/PyAV/installation.html for full installation instructions

5. With virtual env active, install PyAV and any other requirements
    - pip install -r requirements.txt