Setting up locations
====================

**All commands should be run in DM (Direct Message) to Arceus**

Alerts can be set against a channel & area*, but also set against a
defined location of your choosing. You may set up as many locations as
you like, but may only have one location active at a given point.

\**For London, alerts cannot be set up for channel / area\*

Setup locations
~~~~~~~~~~~~~~~

The command to add a new location is:

``!location add name=<name> coord=<coords> distance=<distance>``

coordinates must be supplied in this format ``lat,lon``, for example:

``!location add name=work coord=51.503129,-0.118659 distance=2``

This will create a location at that location with a nickname of work,
and when active will send me alerts when Pokemon alert filters are met
AND the distance to my location is less than 2km.

You can use any name you like, except “all” (this is used to reference
all locations in code) and must be unique.

There is a max distance setting applied on the server, so whilst you can
enter as high a distance as you like, if greater than the system max
distance, will use the system setting. We have done this as we will
change the max setting based on numbers of alerts going out.

Set location active
^^^^^^^^^^^^^^^^^^^

You’ve set up 1 or more locations using the guide above. To set a
location as active:

``!location set <name>``

Using my example above, I would type ``!location set work`` to make that
location active. Please note, adding a location does not automatically
set it active, so you need to do this too. You can have no locations
active (this will mute all your alerts without channel/area) or you can
have 1 location active. Never more than 1.

When you set a location active, all others locations will be set
inactive.

Show locations
^^^^^^^^^^^^^^

``!location show`` will return a table of all your locations:

::

    NAME   |LATITUDE |LONGITUDE |DISTANCE |ACTIVE
    -------+---------+----------+---------+------
    home   |55.4573  |-0.396158 |1.0      |false 
    london |51.5083  |-0.095649 |2.0      |false 
    work   |52.6889  |-0.452083 |1.0      |true  

This shows that my work location is currently active.

Remove location(s)
~~~~~~~~~~~~~~~~~~

``!location remove <name>``

So to remove my location I set up for work - ``!location remove work``

If you want to remove all locations, type ``!location remove all``

Mute locations
~~~~~~~~~~~~~~

If you want to mute alerts for all locations, just type
``!location mute``

Switching between location based and channel/area based alerts
--------------------------------------------------------------

If you have already got alerts set up for a channel or area, you can
remove the channel & area and switch them to being location based. To do
so:

``!channel remove <ID>`` or ``!channel remove all``

To add switch back to using channel & Area for your alerts:

``!channel enable <id> channel=<channel> area=<area>``, ie
``!channel enable 12345 channel=Brighton area=Patcham``