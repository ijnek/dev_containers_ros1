FROM ros:noetic-desktop

# Update all packages
RUN apt update && apt upgrade -y

# Install extra packages
RUN apt install gdb -y

# Rosdep update
RUN rosdep update

# Source the ROS noetic setup file
RUN echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
