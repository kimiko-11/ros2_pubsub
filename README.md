ROS 2 Pub-Sub Example (Python)
This is a minimal ROS 2 package written in Python that demonstrates a basic Publisher-Subscriber model using rclpy

It publishes "Hello World" messages every second and listens to them on another node — perfect for beginners learning ROS 2 concepts.

Project Structure
py_pubsub/ ├── py_pubsub/ │ ├── publisher_node.py │ ├── subscriber_node.py ├── images/ │ ├── publisher_output.png │ └── rqt_graph.png ├── package.xml ├── setup.py ├── setup.cfg ├── README.md

Nodes
Node Name	Description
minimal_publisher	Publishes a string message on /chatter
minimal_subscriber	Listens to /chatter and prints messages
🚀 Run Instructions
🔧 Build the Workspace
cd ~/ros2_ws
colcon build
source install/setup.bash
🗣️ Run the Publisher
ros2 run py_pubsub talker

👂 Run the Subscriber
ros2 run py_pubsub listener
Visual Output
🖥️ Publisher Terminal Output

📈 rqt_graph Visualization

🛠 Requirements
Ubuntu 22.04 with ROS 2 (Humble recommended)

Python 3.10+

WSL2 (if on Windows)

rclpy, colcon, and rqt_graph
