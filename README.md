# TECHIN 517

Labs for TECHIN 517 robotics studio 2.

The labs are located in the [wiki](https://github.com/GIXLabs/TECHIN517/wiki) of this repo.

The code has everything you'll need for the Fetch robotics ROS Noetic workspace.

To get started, clone this repo:

```bash
git clone https://github.com/GIXLabs/TECHIN517.git
```

Go into the fetch_ws and install the class code:

```bash
cd fetch_ws
```

```bash
./install_fetch_ws.sh
```
## Prepare work

1. open dev container fetch_ws in Vscode: "Reopen in Container" option, there will be "Dev Container:TECHIN517Fetch" at the bottom left of Vscode

2.Run the roscore in one terminal:
```bash
roscore
```

3. Run the Gazebo in another terminal:

Test that the package built successfully by running:

```bash
rosrun applications hello_world.py
```
You should see:
```bash
/hello_world main:8: Hello world!
```
```bash
/hello_world main:8: Hello world!
```
Then run:
```bash
roslaunch fetch_gazebo playground.launch
```
4. run Moveit:
```bash
roslaunch fetch_moveit_config move_group.launch
```
Then make script executable and run it:
```bash
chmod +x /fetch_ws/src/fetch-picker/applications/scripts/check_cart_pose.py
rosrun applications check_cart_pose.py plan 0.5 0 1
```





