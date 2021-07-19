# choreonoid_ros_setup
## How to setup
1. Install vcstool
```
sudo apt install -y python3-vcstool
```
2. Clone repositories
```
mkdir src
vcs import < choreonoid.repos
```
3. Build
```
catkin config --cmake-args -DBUILD_CHOREONOID_EXECUTABLE=OFF -DUSE_PYTHON3=OFF -DCMAKE_BUILD_TYPE=Release -DBUILD_WRS2018=ON -DBUILD_COMPETITION_PLUGIN=ON -DBUILD_MULTICOPTER_PLUGIN=ON -DBUILD_MULTICOPTER_SAMPLES=ON
catkin build
```
