# rgbd

 This is for testing rgbd slam in ros kinetic in xenial
 
 PART 1 : SETTING UP WORKSPACE
 
Create a rgbd workspace : mkdir rgbd

Then go into the folder : cd rgbd

Create a source folder : mkdir src

Go into source folder : cd src

Cloning into rgbd workspace src folder : git clone https://github.com/felixendres/rgbdslam_v2

Other clones i did (optional) : g2o , cvpr-tools/cvpr-cuda (vision.tum), pcl-pcl-1.8.0 , ptam-wrapper , rgbd_benchmark 

Now export the ros package path :export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:`pwd`

Go back to workspace directory : cd..

Source the rosdistro files: source /opt/ros/kinetic/setup.bash

Initiate catkin : catkin init

Build workspace : catkin build

Update rosdep : update rosdep

Rosmake the package : rosmake rgbdslam

Source setup file : source devel/setup.bash

PART 2 : TESTING 

install cython : sudo apt-get install cython

go to test folder : cd src/rgbdslam_v2-kinetic/test

There is a readme file that provides further information of the steps ahead
