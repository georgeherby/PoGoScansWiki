***********
Raid Alerts
***********

.. contents:: :local:

If you want to set up alerts for raids going on in areas near you, initiate a conversation with Dialga by typing into bot-commands:

::

    !raid
	
This will get Dialga to send you a message. Use this DM window to send all commands. 

Adding Alerts
#############

The following parameters are used for setting up raid alerts:

* **channel** - The discord channel of interest. *Mandatory*.
* **area** - The geofence area of interest OR the name of the gym you want alerting for. *Mandatory*.
* **level** - The minimum level to alert for. *(either level or boss is mandatory)*
* **boss** - Theboss name to alert for. *(either level or boss is mandatory)*
* **egg** - This parameter will indicate whether you want alerting to egg posts or hatched bosses. *Optional*

Example Alert Commands
----------------------

All bosses in Ferring with minimum level of 3

::

    !raid channel=worthing area=Ferring level=3

All eggs in Ferring with minimum level of 5

::

    !raid channel=worthing area=Ferring level=5 egg

All raids in Ferring for Wailmer

::

    !raid channel=worthing area=Ferring boss=wailmer
	
.. note::

	You cannot include the egg parameter for boss alerts, because the boss is not known until the egg hatches!
	
All bosses at the "Kick Boxing Club Mural" gym

::

    !raid channel=brighton gym=Kick Boxing Club Mural level=1

All eggs at the "Kick Boxing Club Mural" gym

::

    !raid channel=brighton gym=Kick Boxing Club Mural level=1 egg

All raids at "St Andrews Church" for Wailmer

::

    !raid channel=South gym=St Andrews Church boss=wailmer
	
.. note::

	When using gyms for raid alerts, make sure the name you use in your command matches the name in the discord posts EXACTLY. If it does not, you'll not receive any alerts for the gym.

Showing Alerts
--------------

This is to allow you to see all the raids that you have set up and this
is your reference for the raid id (left most column)

::

    !raid show

Returns:

::

    RAID ID |CHANNEL  |AREA/GYM     |BOSS/EGG   |LEVEL |MUTED
    --------+---------+-------------+-----------+------+-----
    1       |Worthing |All          |All Eggs   |4     |     
    66      |Worthing |Ilex Way Park|All Eggs   |5     |     
    28      |Worthing |All          |All Bosses |4     |     
    34      |Worthing |All          |Machamp    |-     | 

There are a few extra options for this command (always in ascending
order)

::

    !raid show boss        Returns a list sorted by Boss, Channel

Removing, Muting Or Unmuting Alerts
-----------------------------------

By ID
~~~~~~~~~~~~

First run show command above and note the raid alert id for the record you
want to remove

Once you have the raid alert id, use this command to remove, mute or unmute the alert

::

    !raid remove 32        ------ 32 being the ID you want to remove
	!raid mute 32        ------ 32 being the ID you want to mute
	!raid unmute 32        ------ 32 being the ID you want to unmute

All alerts
~~~~~~~~~~~~~~~~~

::

    !raid remove all       ------ This will remove all raid alerts
	!raid mute all       ------ This will mute all raid alerts
	!raid unmute all       ------ This will unmute all raid alerts

By Location
~~~~~~~~~~~~~~~~~~

You can remove, mutye or unmute all alerts for a channel or an area within a channel:

::

    !raid remove channel=MidSussex
    !raid remove channel=CentralEast area=Covent Garden
	
::

    !raid mute channel=MidSussex
    !raid mute channel=CentralEast area=Covent Garden
	
::

    !raid unmute channel=MidSussex
    !raid unmute channel=CentralEast area=Covent Garden

.. note::

	If removing by area, channel is still required.
