## Robot Package Template

This is a GitHub template. You can make your own copy by clicking the green "Use this template" button.

It is recommended that you keep the repo/package name the same, but if you do change it, ensure you do a "Find all" using your IDE (or the built-in GitHub IDE by hitting the `.` key) and rename all instances of `etug` to whatever your project's name is.

Note that each directory currently has at least one file in it to ensure that git tracks the files (and, consequently, that a fresh clone has direcctories present for CMake to find). These example files can be removed if required (and the directories can be removed if `CMakeLists.txt` is adjusted accordingly).

go into workspace

--if any files are added
colcon build --symlink-install

--for any terminal that needs to run rviz or run ros commands in this workspace
source install/setup.bash

--open rviz (can't use vscode terminal to launch rviz)
rviz2

--if any files are changed
ros2 launch etug rsp.launch.py


