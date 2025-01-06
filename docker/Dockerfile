FROM rwthika/ros2:humble

WORKDIR /stanley_controller_cpp

COPY ../ /stanley_controller_cpp

RUN apt-get update && apt-get install -y \
    libeigen3-dev \
    python3-matplotlib \
    python3-dev \
    && rm -rf /var/lib/apt/lists/*
