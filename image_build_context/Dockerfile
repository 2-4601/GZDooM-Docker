FROM ubuntu

# Install required packages
RUN apt-get update && \
    apt-get install -y \
      cmake \
      g++ \
      git \
      libbz2-dev \
      libfluidsynth-dev \
      libgl1-mesa-dev \
      libglew-dev \
      libgme-dev \
      libgtk-3-dev \
      libjpeg-dev \
      libmpg123-dev \
      libopenal-dev \
      libsdl1.2-dev \
      libsdl2-dev \
      libsndfile1-dev \
      libwildmidi-dev \
      nasm \
      make \
      tar \
      timidity \
      zlib1g-dev \
    && rm -rf /var/lib/apt/lists/*

# Initial settings
WORKDIR /gzdoom

ADD build_gzdoom.sh .

CMD ["./build_gzdoom.sh"]
