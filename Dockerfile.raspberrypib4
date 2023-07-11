FROM debian:buster

RUN apt-get update && \
    apt-get install -y ffmpeg \
    python3 \
    python3-pip \
    libatlas-base-dev \
    git \
    libtiff5-dev \
    libjpeg62-turbo-dev \
    libopenjp2-7-dev \
    zlib1g-dev \
    libfreetype6-dev \
    liblcms2-dev \
    libwebp-dev \
    tcl8.6-dev \
    tk8.6-dev \
    python3-tk \
    python3-numpy \
    python3-pil \
    python3-sklearn \
    libharfbuzz-dev \
    libfribidi-dev \
    libxcb1-dev

RUN pip3 install --no-cache-dir --upgrade pip && \
        pip3 install --no-cache-dir --no-deps --extra-index-url https://www.piwheels.org/simple \
        tqdm \
        imageio \
        imageio-ffmpeg \
        tflite-runtime
RUN pip3 install git+https://github.com/vaik-info/vaik-video-classification-tflite-inference.git --no-deps --extra-index-url https://www.piwheels.org/simple