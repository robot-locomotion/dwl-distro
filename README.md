The Dynamic Whole-body Locomotion library (DWL) distro
===============================================

<img align="left" height="240" src="https://imgur.com/SkeMizm.png"/> 

## <img align="center" height="20" src="https://i.imgur.com/vAYeCzC.png"/> Introduction

This distro contains all the dwl package under development. The *Dynamic Whole-body Locomotion* library (DWL) implements a set of functionalities to develop, design, and deploy motion planning, control and perception algorithms for legged locomotion. DWL has different modules such as: kinematics, dynamics, solvers (tree-search, optimization, etc), and environment descriptions. All these tools are designed for both fast prototyping and deployment thanks to its c++ implementation and Python bindings. The DWL toolbox can be used in various software frameworks such as ROS and LCM, and for real-time control and planning.

DWL was developed by Carlos Mastalli at [Dynamic Legged Systems lab (DLS)](http://www.iit.it/en/advr-labs/dynamic-legged-systems.html), Istituto Italiano di Tecnologia, Italy. The DWL is core toolbox used along of various software of the DLS lab at IIT.

| [![](https://i.imgur.com/BT7fRCU.gif)](https://www.youtube.com/watch?v=ENHvCGrnr2g&t=2s) | [![](https://i.imgur.com/4kKhryj.gif)](https://www.youtube.com/watch?v=KI9x1GZWRwE)
|:-------------------------:|:-------------------------:|
| [![](https://i.imgur.com/yXTtxUK.gif)](https://www.youtube.com/watch?v=ArV2yh7KSfE) | [![](https://i.imgur.com/RKe3sNo.gif)](https://www.youtube.com/watch?v=KI9x1GZWRwE)
|||



The source code is released under a [BSD 3-Clause license](LICENSE).

**Author: Carlos Mastalli, carlos.mastalli@laas.fr<br />
With support from the Dynamic Legged Systems lab at Istituto Italiano di Tecnologia<br />**



[![License BSD-3-Clause](https://img.shields.io/badge/license-BSD--3--Clause-blue.svg?style=flat)](https://tldrlegal.com/license/bsd-3-clause-license-%28revised%29#fulltext)
[![Build Status](https://api.travis-ci.org/robot-locomotion/dwl.svg?branch=master)](https://api.travis-ci.org/repositories/robot-locomotion/dwl.svg)




## <img align="center" height="20" src="https://i.imgur.com/x1morBF.png"/> Building

To build dwl-distro from source code, you first need to install the dwl dependencies. We recommend you to install them using the install_deps.sh script. The INSTALL_DEPS_PREFIX defines the folder where is installed its dependencies (usually /usr/local for linux machines). However you can install them in your local folder. 

Once dependencies are installed, you can build the dwl-distro with ROS. Copy the entired distro into the src directory of your catkin workspace, and compile it:

    cd your_ros_workspace/
    catkin_make -DCMAKE_INSTALL_PREFIX=${/dwl/installation/path} -DINSTALL_DEPS_PREFIX=${/your/dependencies/path}

Finally you can generate the Python bindings and Doxygen documentation by doing:

   cmake -DDWL_WITH_PYTHON=True -DDWL_WITH_DOC=True ../



## <img align="center" height="20" src="https://i.imgur.com/x1morBF.png"/> Installation

You can install the dwl-distro as any catkin project.



## <img align="center" height="20" src="http://www.pvhc.net/img205/oohmbjfzlxapxqbpkawx.png"/> Publications


* C. Mastalli, I. Havoutis, M. Focchi, D. G. Caldwell, C. Semini, [Motion planning for challenging locomotion: a study of decoupled and coupled approaches](https://hal.archives-ouvertes.fr/hal-01649836v1), IEEE International Conference on Robotics and Automation (ICRA), 2017
* B. Aceituno-Cabezas, C. Mastalli, H. Dai, M. Focchi, A. Radulescu, D. G. Calwell, J. Cappelletto, J. C. Griego, G. Fernardez, C. Semini, [Simultaneous Contact, Gait and Motion Planning for Robust Multi-Legged Locomotion via MICP](http://ieeexplore.ieee.org/document/8141917/), IEEE Robotics and Automation Letters  (RAL), 2017
* C. Mastalli, M. Focchi, I. Havoutis, A. Radulescu, D. G. Caldwell, C. Semini, [Trajectory and Foothold Optimization using Low-Dimensional Models for Rough Terrain Locomotion](https://old.iit.it/images/stories/advanced-robotics/hyq_files/publications/mastalli17icra.pdf), IEEE International Conference on Robotics and Automation (ICRA), 2017
* C. Mastalli, I. Havoutis, M. Focchi, D. G. Caldwell, C. Semini, [Hierarchical Planning of Dynamic Movements without Scheduled Contact Sequences](http://iit.it/images/stories/advanced-robotics/hyq_files/publications/icra16mastalli.pdf), IEEE International Conference on Robotics and Automation (ICRA), 2016
* C. Mastalli, A. Winkler, I. Havoutis, D. G. Caldwell, C. Semini, [On-line and On-board Planning and Perception for Quadrupedal Locomotion](http://iit.it/images/stories/advanced-robotics/hyq_files/publications/mastalli15tepra.pdf), IEEE International Conference on Technologies for Practical Robot Applications (TEPRA), 2015
* A. Winkler, C. Mastalli, I. Havoutis, M. Focchi, D. G. Caldwell, C. Semini, [Planning and Execution of Dynamic Whole-Body Locomotion for a Hydraulic Quadruped on Challenging Terrain](http://iit.it/images/stories/advanced-robotics/hyq_files/publications/winkler15icra.pdf), IEEE International Conference on Robotics and Automation (ICRA), 2015
