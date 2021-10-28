# gazebo_sim
Robot-agnostic simulated environment in Gazebo

## Usage
To start a simulation world in gazebo use the following command:

```
roslaunch gazebo_sim start_sim_env.launch
```

The launch file also accepts some arguments. The most relevant are:

| arg_name | description | arg_type | default |
| ----- | ----- | ----- | ----- |
| world | name of the world to be spawned | string | brsu |
| paused | Start Gazebo in a paused state | bool | false |
| gui | Start the Gazebo GUI | bool | true |

For example, to start the simulation with the `simple_two_rooms` world without the Gazebo GUI, use the following command:

```
roslaunch gazebo_sim start_sim_env.launch world:=simple_two_rooms gui:=false
```

## Additional Resources:

### Gazebo worlds
1. [AWS Robotics worlds](https://github.com/aws-robotics) 
    1. [AWS RoboMaker Small House World](https://github.com/aws-robotics/aws-robomaker-small-house-world)
    2. [AWS RoboMaker Small Warehouse World](https://github.com/aws-robotics/aws-robomaker-small-warehouse-world)
    3. ... and several others.
2. [Ignitionrobotics Worlds](https://app.ignitionrobotics.org/fuel/worlds)
3. [Gazebo models and worlds collection](https://github.com/chaolmu/gazebo_models_worlds_collection)

### Gazebo object models
1. [YCB dataset reconstructed objects](http://ycb-benchmarks.s3-website-us-east-1.amazonaws.com/)
2. [Ignitionrobotics models](https://app.ignitionrobotics.org/fuel/models)
