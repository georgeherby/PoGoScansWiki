*********
Locations
*********

In order to get alerts for spawns within a certain distance of you (see :doc:`Setting Up Location Alerts </arceus/location_alerts>`), you must set up locations. You can store a list of locations to switch between (add and remove), but may only have one active location at a time (chosen by setting). 
You can switch your active location as you wish, but you must type the command; there is no tracking.

.. contents:: :local:

Viewing Locations
#################

::

	!location show
	
Shows a list of your saved locations, and shows which is active. It’s the go-to to see what’s going on with locations.

.. image:: location_show.PNG

Adding/Removing Locations
############################

::

	!location add name=<name> coord=<coords>
	
For example ``!location add name=needle coord=51.5085,-0.1204``

Adds a new location. 

.. note::

	* <name> should be alphanumeric - spaces won’t be accepted.
	* The command is coord, not coords!
	* <coords> should be in decimal notation only (51.xxx..,-0.xxx..).
	* No spaces around the comma between coords, nor either side of any of the = in the command.
	* Even if you only add one location, it doesn’t automatically become active (see Setting/Unsetting Locations below).

::

	!location remove <name>

For example !location remove needle

Removes a location by its name as stored at ``!location show``.

::

	!location remove all
	
Removes all stored locations; start afresh!

Setting/Unsetting Locations
###########################

::

	!location set needle
	
Sets a location to active by its name as stored at ``!location show``. All other locations become inactive.

::

	!location mute
	
Sets all locations to inactive.
