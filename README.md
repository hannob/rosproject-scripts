ROS sanitizer scripts
=====================

These scripts were created in a project intending to test
the ROS software with the compiler sanitizers available
in gcc and clang.

You can find a report about the project
[here](https://github.com/hannob/rosproject-scripts/blob/master/report/rosreport.pdf).

build_catkin_module
===================

Compiles and runs tests with a sanitizer.

Usage:
```
./build_catkin_module [sanitizer] [github repo] [module] [path_optional]
```

Repository checkouts, build dirs and logs are all stored in /catkin.

Example call:
```
./build_catkin_module $SANITIZER ros_comm topic_tools tools
```

This will build the package topic_tools, which is in the ROS repository
ros_comm in the subdirectory tools.

call_catkin
===========

This simply contains example calls for all packages within the ROS
github repositories.

copyright/license
=================

All scripts here are provided under a CC0 license, meaning you're
free to do with them whatever you like.

Created by [Hanno Böck](https://hboeck.de)
