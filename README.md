# action_tutorials_cpp

## First of all you need to go through your working space and after that creade the a package

```
os2 pkg create --dependencies action_tutorials_interfaces rclcpp rclcpp_action rclcpp_components -- action_tutorials_cpp
```
## after taht you need to follow the instraction according to the changes at the coding part of the Fibonacci_action_server.cpp and the visibility_control.h. If you can not find this files you might use the "touch" function to create that files and after that add the main coding parts that  you might need to use.
## after that you need to go to the working space and there you need to run the "colcon build" function and then you will run the other code that will help you to run the action
```
colcon buil
```

```
[0.594s] WARNING:colcon.colcon_core.package_identification:Failed to parse ROS package manifest in 'tutorial_interfaces': Error(s) in package 'tutorial_interfaces/package.xml':
The package "tutorial_interfaces" must not "build_depend" on a package with the same name as this package
The package "tutorial_interfaces" must not "build_export_depend" on a package with the same name as this package
The package "tutorial_interfaces" must not "exec_depend" on a package with the same name as this package
[0.925s] WARNING:colcon.colcon_core.package_selection:Some selected packages are already built in one or more underlay workspaces:
	'examples_rclpy_minimal_service' is in: /opt/ros/humble
	'std_msgs' is in: /opt/ros/humble
	'demo_nodes_cpp' is in: /opt/ros/humble
	'ament_cmake_auto' is in: /opt/ros/humble
	'examples_rclcpp_minimal_action_client' is in: /opt/ros/humble
	'rclcpp_action' is in: /opt/ros/humble
	'rosbag2_transport' is in: /opt/ros/humble
	'ros2launch' is in: /opt/ros/humble
	'rqt_action' is in: /opt/ros/humble
	'demo_nodes_cpp_native' is in: /opt/ros/humble
	'examples_rclcpp_multithreaded_executor' is in: /opt/ros/humble
	'quality_of_service_demo_cpp' is in: /opt/ros/humble
	'ament_index_cpp' is in: /opt/ros/humble
	'sros2_cmake' is in: /opt/ros/humble
	'rcpputils' is in: /opt/ros/humble
	'dummy_robot_bringup' is in: /opt/ros/humble
	'rqt_msg' is in: /opt/ros/humble
	'examples_rclpy_minimal_action_client' is in: /opt/ros/humble
	'ament_cmake_ros' is in: /opt/ros/humble
	'qt_gui_cpp' is in: /opt/ros/humble
	'rqt_graph' is in: /opt/ros/humble
	'rqt_gui' is in: /opt/ros/humble
	'launch_testing_ament_cmake' is in: /opt/ros/humble
	'examples_rclpy_executors' is in: /opt/ros/humble
	'lifecycle' is in: /opt/ros/humble
	'sros2' is in: /opt/ros/humble
	'rqt_py_console' is in: /opt/ros/humble
	'rqt_shell' is in: /opt/ros/humble
	'robot_state_publisher' is in: /opt/ros/humble
	'quality_of_service_demo_py' is in: /opt/ros/humble
	'eigen3_cmake_module' is in: /opt/ros/humble
	'common_interfaces' is in: /opt/ros/humble
	'rqt_srv' is in: /opt/ros/humble
	'pluginlib' is in: /opt/ros/humble
	'ros_environment' is in: /opt/ros/humble
	'rqt_topic' is in: /opt/ros/humble
	'tlsf_cpp' is in: /opt/ros/humble
	'rqt_reconfigure' is in: /opt/ros/humble
	'builtin_interfaces' is in: /opt/ros/humble
	'logging_demo' is in: /opt/ros/humble
	'rcutils' is in: /opt/ros/humble
	'action_tutorials_interfaces' is in: /opt/ros/humble
	'topic_monitor' is in: /opt/ros/humble
	'rviz_default_plugins' is in: /opt/ros/humble
	'launch_xml' is in: /opt/ros/humble
	'launch_ros' is in: /opt/ros/humble
	'turtlesim' is in: /opt/ros/humble
	'rclcpp' is in: /opt/ros/humble
	'rosidl_runtime_py' is in: /opt/ros/humble
	'image_tools' is in: /opt/ros/humble
	'message_filters' is in: /opt/ros/humble
	'rclcpp_components' is in: /opt/ros/humble
	'rqt_plot' is in: /opt/ros/humble
	'examples_rclcpp_minimal_action_server' is in: /opt/ros/humble
	'rpyutils' is in: /opt/ros/humble
	'examples_rclcpp_minimal_publisher' is in: /opt/ros/humble
	'urdf' is in: /opt/ros/humble
	'rqt_service_caller' is in: /opt/ros/humble
	'kdl_parser' is in: /opt/ros/humble
	'launch_testing' is in: /opt/ros/humble
	'rosbag2_cpp' is in: /opt/ros/humble
	'examples_rclpy_minimal_client' is in: /opt/ros/humble
	'examples_rclcpp_minimal_subscriber' is in: /opt/ros/humble
	'geometry2' is in: /opt/ros/humble
	'intra_process_demo' is in: /opt/ros/humble
	'launch' is in: /opt/ros/humble
	'rosidl_default_generators' is in: /opt/ros/humble
	'composition' is in: /opt/ros/humble
	'class_loader' is in: /opt/ros/humble
	'rcl_interfaces' is in: /opt/ros/humble
	'rclcpp_lifecycle' is in: /opt/ros/humble
	'rqt_gui_cpp' is in: /opt/ros/humble
	'demo_nodes_py' is in: /opt/ros/humble
	'ament_cmake_core' is in: /opt/ros/humble
	'rqt_publisher' is in: /opt/ros/humble
	'sensor_msgs' is in: /opt/ros/humble
	'examples_rclpy_minimal_publisher' is in: /opt/ros/humble
	'rviz2' is in: /opt/ros/humble
	'action_tutorials_py' is in: /opt/ros/humble
	'rcl_lifecycle' is in: /opt/ros/humble
	'action_tutorials_cpp' is in: /opt/ros/humble
	'ros2cli_common_extensions' is in: /opt/ros/humble
	'ament_cmake_pytest' is in: /opt/ros/humble
	'rqt_py_common' is in: /opt/ros/humble
	'pendulum_msgs' is in: /opt/ros/humble
	'rqt_console' is in: /opt/ros/humble
	'dummy_map_server' is in: /opt/ros/humble
	'examples_rclcpp_minimal_timer' is in: /opt/ros/humble
	'ament_cmake_gmock' is in: /opt/ros/humble
	'rosbag2' is in: /opt/ros/humble
	'dummy_sensors' is in: /opt/ros/humble
	'rclpy' is in: /opt/ros/humble
	'rosidl_default_runtime' is in: /opt/ros/humble
	'launch_testing_ros' is in: /opt/ros/humble
	'examples_rclpy_minimal_action_server' is in: /opt/ros/humble
	'rosbag2_compression' is in: /opt/ros/humble
	'ament_cmake' is in: /opt/ros/humble
	'examples_rclcpp_minimal_client' is in: /opt/ros/humble
	'ament_lint_common' is in: /opt/ros/humble
	'examples_rclcpp_minimal_service' is in: /opt/ros/humble
	'rosbag2_storage_default_plugins' is in: /opt/ros/humble
	'rosbag2_storage' is in: /opt/ros/humble
	'pendulum_control' is in: /opt/ros/humble
	'tlsf' is in: /opt/ros/humble
	'ament_lint_auto' is in: /opt/ros/humble
	'launch_yaml' is in: /opt/ros/humble
	'zstd_vendor' is in: /opt/ros/humble
	'examples_rclpy_minimal_subscriber' is in: /opt/ros/humble
	'ament_index_python' is in: /opt/ros/humble
	'geometry_msgs' is in: /opt/ros/humble
	'ament_cmake_gtest' is in: /opt/ros/humble
	'examples_rclcpp_minimal_composition' is in: /opt/ros/humble
If a package in a merged underlay workspace is overridden and it installs headers, then all packages in the overlay must sort their include directories by workspace order. Failure to do so may result in build failures or undefined behavior at run time.
If the overridden package is used by another package in any underlay, then the overriding package in the overlay must be API and ABI compatible or undefined behavior at run time may occur.

If you understand the risks and want to override a package anyways, add the following to the command line:
	--allow-overriding action_tutorials_cpp action_tutorials_interfaces action_tutorials_py ament_cmake ament_cmake_auto ament_cmake_core ament_cmake_gmock ament_cmake_gtest ament_cmake_pytest ament_cmake_ros ament_index_cpp ament_index_python ament_lint_auto ament_lint_common builtin_interfaces class_loader common_interfaces composition demo_nodes_cpp demo_nodes_cpp_native demo_nodes_py dummy_map_server dummy_robot_bringup dummy_sensors eigen3_cmake_module examples_rclcpp_minimal_action_client examples_rclcpp_minimal_action_server examples_rclcpp_minimal_client examples_rclcpp_minimal_composition examples_rclcpp_minimal_publisher examples_rclcpp_minimal_service examples_rclcpp_minimal_subscriber examples_rclcpp_minimal_timer examples_rclcpp_multithreaded_executor examples_rclpy_executors examples_rclpy_minimal_action_client examples_rclpy_minimal_action_server examples_rclpy_minimal_client examples_rclpy_minimal_publisher examples_rclpy_minimal_service examples_rclpy_minimal_subscriber geometry2 geometry_msgs image_tools intra_process_demo kdl_parser launch launch_ros launch_testing launch_testing_ament_cmake launch_testing_ros launch_xml launch_yaml lifecycle logging_demo message_filters pendulum_control pendulum_msgs pluginlib qt_gui_cpp quality_of_service_demo_cpp quality_of_service_demo_py rcl_interfaces rcl_lifecycle rclcpp rclcpp_action rclcpp_components rclcpp_lifecycle rclpy rcpputils rcutils robot_state_publisher ros2cli_common_extensions ros2launch ros_environment rosbag2 rosbag2_compression rosbag2_cpp rosbag2_storage rosbag2_storage_default_plugins rosbag2_transport rosidl_default_generators rosidl_default_runtime rosidl_runtime_py rpyutils rqt_action rqt_console rqt_graph rqt_gui rqt_gui_cpp rqt_msg rqt_plot rqt_publisher rqt_py_common rqt_py_console rqt_reconfigure rqt_service_caller rqt_shell rqt_srv rqt_topic rviz2 rviz_default_plugins sensor_msgs sros2 sros2_cmake std_msgs tlsf tlsf_cpp topic_monitor turtlesim urdf zstd_vendor

This may be promoted to an error in a future release of colcon-override-check.
[0.926s] ERROR:colcon:colcon build: Duplicate package names not supported:
- action_tutorials_cpp:
  - action_tutorials_cpp
  - ros2/demos/action_tutorials/action_tutorials_cpp
- action_tutorials_interfaces:
  - action_tutorials_interfaces
  - ros2/demos/action_tutorials/action_tutorials_interfaces
```
## and then you need to run the ros2 function

```
ros2 run action_tutorials_cpp fibonacci_action_client
```
