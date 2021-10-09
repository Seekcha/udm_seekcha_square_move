# udm_seekcha_square_move


This package contains the TP4 Part 3 package. It allows you to describe a square with the Turtlebot3 by calling the move_base / goal service.

## Installation
The package need to be install in your catkin workspace.
```
cd catkin_ws/src
git clone https://github.com/Seekcha/udm_seekcha_square_move.git
catkin build
cd ..
source devel/setup.bash
```

## Execution
Open world.launch in first terminal:
```
source devel/setup.bash
export TURTLEBOT3_MODEL=waffle_pi
roslaunch turtlebot3_gazebo turtlebot3_world.launch
```

Open navigation.launch in second terminal:
```
source devel/setup.bash
export TURTLEBOT3_MODEL=waffle_pi
roslaunch udm_seekcha_square_move turtlebot3_navigation.launch map_file:=$HOME/map.yaml

```

Open navigation.launch in third terminal:
```
source devel/setup.bash
export TURTLEBOT3_MODEL=waffle_pi
rosrun udm_seekcha_square_move movebase_square.py

```



