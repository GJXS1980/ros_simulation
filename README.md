#### ros_simulation
编译步骤：
```bash
mkdir -p ~/ros_simulation/src
cd ~/ros_simulation/src
git clone https://github.com/GJXS1980/ros_simulation.git
cd ros_simulation/gazebo_ros_pkgs
git config core.sparsecheckout true
echo gazebo_ros_control/ >> .git/info/sparse-checkout
git checkout
rosdep install --from-paths . -i -y
cd ~/ros_simulation
catkin_make
echo "source ~/ros_simulation/devel/setup.bash" >> ~/.bashrc 
source ~/.bashrc
```













