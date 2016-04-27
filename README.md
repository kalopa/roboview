RoboView
========

RoboView is a GTK+ application for showing robots or objects in a two-dimensional space.
The viewer listens on a well-known TCP port (1702) for text messages for each of the objects.
It is invoked with a background map image.
The code doesn't detect collisions or do anything other than map (in real-time) the x,y
location and orientation of a range of objects.
The objects themselves are also provided as a range of bitmaps representing different angles.
