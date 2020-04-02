^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package realsense_gazebo_plugin
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.0.1 (2020-04-02)
------------------
* Fixed dependencies missing in package.xml
* Updated maintainer and install target
* Update README.md
* Merge pull request `#39 <https://github.com/LCAS/realsense_gazebo_plugin/issues/39>`_ from ManMan88/master
  fix issue `#37 <https://github.com/LCAS/realsense_gazebo_plugin/issues/37>`_
* Merge pull request `#45 <https://github.com/LCAS/realsense_gazebo_plugin/issues/45>`_ from Awesome-Technologies/gazebo-compat
  Keep compatibility with earlier Gazebo version
* Keep compatibility with earlier Gazebo version
* Issue `#37 <https://github.com/LCAS/realsense_gazebo_plugin/issues/37>`_ - fix support for multiple cameras
* Merge pull request `#36 <https://github.com/LCAS/realsense_gazebo_plugin/issues/36>`_ from marcoesposito1988/patch-2
  Overridable camera_name arg of depth_proc.launch
* Overridable camera_name arg of depth_proc.launch
  Doing so allows inclusion in external launch files using other cameras
* Merge pull request `#35 <https://github.com/LCAS/realsense_gazebo_plugin/issues/35>`_ from marcoesposito1988/patch-1
  Catkin package.xml v2, add missing dependency
* Catkin package.xml v2, add missing dependency
* Fix depth processing
  Broken after `#25 <https://github.com/LCAS/realsense_gazebo_plugin/issues/25>`_ fix.
  Had to rename the topics properly for the
  depth processing node.
  Solves `#32 <https://github.com/LCAS/realsense_gazebo_plugin/issues/32>`_
* Enable multiple R200 to co-exist in one world
  This was previously broken because all R200 plugins would publish
  under the same topics and overwrite each other. This is now fixed
  and there is a demo launch file to show that it works :)
  Solves `#25 <https://github.com/LCAS/realsense_gazebo_plugin/issues/25>`_
* Remove fake origin -> color TF publisher
* Compute focal from rendering's horizontal FOV
  Fixes `#28 <https://github.com/LCAS/realsense_gazebo_plugin/issues/28>`_
* Simplify camera & encoding identification
* Add dependency to image_pipeline in package manifest
* Add important note on supported ROS/Gazebo versions
  Addresses the recurrent issues reporting that the master branch
  fails to compile on ROS Kinetic + Gazebo 7.
  Solves `#20 <https://github.com/LCAS/realsense_gazebo_plugin/issues/20>`_
* Merge pull request `#17 <https://github.com/LCAS/realsense_gazebo_plugin/issues/17>`_ from felixvd/patch-1
  Add prefix to URDF to allow multiple cameras in the same scene
* Update parent xacro to fit the new macro
  This also serves an example of how to use the other file..
* Add prefix and parent to RS200 macro
  This allows the use of multiple cameras and is cleaner to insert.
* Update README.md
* Merge pull request `#13 <https://github.com/LCAS/realsense_gazebo_plugin/issues/13>`_ from shylent/fix-gtest-link-error
  test_realsense_streams: Fix linking error
* CMakeLists.txt: Link test_realsense_streams binary against threading library
* Add a launch file to show usage with ROS
* Fix build for Gazebo 9
* Update acknowledgement
* Format URDF
* Merge pull request `#10 <https://github.com/LCAS/realsense_gazebo_plugin/issues/10>`_ from Danfoa/master
  Generation of the Gazebo model in URDF format
* small correction to color frame position
* Add realsense urdf description file, to allow loading of camara to `robot_description` parameter, allowing the set up of the camera onto robots and its simulation on gazebo
* Add realsense urdf description file, to allow loading of camara to `robot_description` parameter, allowing the set up of the camera onto robots and its simulation on gazebo
* Merge pull request `#7 <https://github.com/LCAS/realsense_gazebo_plugin/issues/7>`_ from SyrianSpock/support-depth-proc
  Support depth_image_proc
* Add depth_image_proc demo
* Publish camera info for all images including depth
* Merge branch 'publish-depth'
* Update test world to have some depth
* Stream depth image over ROS
* Rename files
* Complete image streams unittests
* Remove debug print
* Update README
* Add first color image stream unittests
* Dispatch image streams correctly between different camera topics
* Implement a basic ROS plugin on top of Gazebo plugin
  Only publishes image streams, and publishes all three streams on the same topic
* Refactor Gazebo plugin
* Fix plugin loading at init
* Make it a Gazebo ROS plugin package
* Add readme
* Add model and world to test it
* Make it build, using Gazebo 7
* Add RealSense plugin from Guilherme Campos Camargo's work
  Doesn't build yet
* Contributors: Daniel Ordonez, Felix von Drigalski, Manuel Stahl, Marco Esposito, Riccardo, Ron Danon, Salah Missri, Salah-Eddine Missri, mlvov
