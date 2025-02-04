# Adapting Task and Joint Weights

The tutorial can be found in [tutorials/kuka_iiwa/cart_pos_ctrl_hls_weights.cpp](https://github.com/ARC-OPT/wbc/blob/master/tutorials/kuka_iiwa/cart_pos_ctrl_hls_weights.cpp), documentation can be found [here](https://arc-opt.github.io/wbc/cart__pos__ctrl__hls__weights_8cpp.html). To run the tutorial, type
```
cd build/tutorials/kuka_iiwa
./cart_pos_ctrl_hls_weights
```

This tutorial shows the effect of modifying the task weights and joint weights. If you set a task weight to zero, the corresponding task variable will assume an arbitrary value (and not the desired setpoint). If you set a joint weight to zero, the corresponding joint will not contribute to the task solution, i.e., its velocity will be zero!

### Adapting the Task Weights

All task weights are set to 1:<br>
<video width="320" height="240" controls>
   <source type="video/mp4"  src="https://raw.githubusercontent.com/ARC-OPT/ARC-OPT/master/videos/task_weights_1.mp4"/>
</video>
Orientation control deactivated (task weights 4,5,6 set to zero): <br>
<video width="320" height="240" controls>
   <source type="video/mp4"  src="https://raw.githubusercontent.com/ARC-OPT/ARC-OPT/master/videos/task_weights_2.mp4"/>
</video>

### Adapting the Joint Weights

All joint weights are set to 1:<br>
<video width="320" height="240" controls>
   <source type="video/mp4"  src="https://raw.githubusercontent.com/ARC-OPT/ARC-OPT/master/videos/joint_weights_1.mp4"/>
</video>
Joint 5 deactivated (joint weight 5 set to zero): <br>
<video width="320" height="240" controls>
   <source type="video/mp4"  src="https://raw.githubusercontent.com/ARC-OPT/ARC-OPT/master/videos/joint_weights_2.mp4"/>
</video>

Please note that the visualization has been done with an external tool and is not part of ARC-OPT. If you want to visualize your system, please refer to the [ROS 2 tutorials](https://arc-opt.github.io/Documentation/tutorials/ros2_introduction.html), which use rviz as visualization.

[[Previous Tutorial]](https://arc-opt.github.io/Documentation/tutorials/vel_using_different_solver.html)[[Back to Main Page]](https://arc-opt.github.io/Documentation)[[Next Tutorial]](https://arc-opt.github.io/Documentation/tutorials/vel_task_hierarchies.html)
