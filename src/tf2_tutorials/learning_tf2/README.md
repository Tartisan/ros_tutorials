## How To Use
```
# tf2 static broadcaster
rosrun learning_tf2 static_turtle_tf2_broadcaster mystaticturtle 0 0 1 0 0 0
rostopic echo /tf_static

# tf2 broadcaster
roslaunch learning_tf2 start_demo.launch

# tf2 message_filter
roslaunch turtle_tf2 turtle_tf2_sensor.launch 
rosrun learning_tf2 message_filter
```

## Reference
[ros wiki: tf2/Tutorials/Learning tf2](http://wiki.ros.org/tf2/Tutorials)

[ros wiki: tf2/Tutorials/Writing a tf2 static broadcaster (C++)](http://wiki.ros.org/tf2/Tutorials/Writing%20a%20tf2%20static%20broadcaster%20%28C%2B%2B%29)

[ros wiki: tf2/Tutorials/Writing a tf2 broadcaster (C++)](http://wiki.ros.org/tf2/Tutorials/Writing%20a%20tf2%20broadcaster%20%28C%2B%2B%29)

[ros wiki: tf2/Using stamped datatypes with tf2::MessageFilter](http://wiki.ros.org/tf2/Tutorials/Using%20stamped%20datatypes%20with%20tf2%3A%3AMessageFilter)

