FROM osrf/ros:melodic-desktop

# Update all packages
RUN apt update && apt upgrade -y

# Install extra packages
RUN apt install gdb -y
RUN apt install git -y

# Rosdep update
RUN rosdep update

# Source the ROS melodic setup file
RUN echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
