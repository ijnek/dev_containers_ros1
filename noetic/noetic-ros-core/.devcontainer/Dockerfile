FROM ros:noetic-ros-core

# Update all packages
RUN apt update && apt upgrade -y

# Install extra packages
RUN apt install build-essential -y
RUN apt install gdb -y
RUN apt install git -y
RUN apt install python3-catkin-tools -y
RUN apt install python3-rosdep -y

# Rosdep
RUN rosdep init
RUN rosdep update

# Source the ROS noetic setup file
RUN echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
