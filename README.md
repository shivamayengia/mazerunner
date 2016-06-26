# Maze Runner

Final Project for Artificial Intelligence 2016-1 class at UNICAMP.

Local navigation of the bibed robot NAO on a V-REP simulation using 
reinforcement learning (Q-Learning).
The desired behavior is for the robot to use its sensors to avoid walls
and attempt to get as close as possible to a tag placed at the kitchen.

## Installing

This project has some dependencies that are not managed by pip.
They must, therefore, be installed manually:

* [V-REP simulator](http://www.coppeliarobotics.com/downloads.html)
* [Choregraphe](https://community.aldebaran.com/en/resources/software) Suite
* Aldebaran NAO [Python SDK](http://doc.aldebaran.com/2-1/dev/python/install_guide.html)

Finally, install MazeRunner:

```shell
python setup.py install --user
```

## Executing the Examples

1. First, start `Choregraph`:
```shell
/opt/Aldebaran\ Robotics/Choregraphe\ Suite\ 2.1/bin/naoqi-bin -p 5000
```

2. Open the V-REP simulator:
```shell
/path/to/vrep/vrep.sh
```
Then open one of the scenes in `mazerunner/scenes` folder and run it.

3. Finally, run one of the examples:
```shell
python mazerunner/examples/simple_walker.py
```
