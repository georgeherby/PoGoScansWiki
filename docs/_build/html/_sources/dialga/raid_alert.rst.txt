Raid Alerts
===========

**All commands should be run in DM (Direct Message) to Dialga**

[TOC]

Add Raids
---------

Channel Wide
~~~~~~~~~~~~

All hatched eggs of a certain *MINIMUM* level

::

    !raid channel=worthing area=Ferring level=5

All unhatched eggs of a certain *MINIMUM* level

::

    !raid channel=worthing area=Ferring level=5 egg

All specific name boss bosses from

::

    !raid channel=worthing area=Ferring boss=wailmer

Specific Gym
~~~~~~~~~~~~

**YOU MUST INCLUDE ``LEVEL=1`` FOR ALL RAIDS. AND ``LEVEL=1 EGG`` FOR
ALL EGGS EVEN WHEN SPECIFYING A SINGLE GYM**

All hatched eggs of a certain *MINIMUM* level

::

    !raid channel=worthing gym=Marine Gardens Restaurant level=5

All unhatched eggs of a certain *MINIMUM* level

::

    !raid channel=worthing gym=Marine Gardens Restaurant level=5 egg

All specific name boss bosses from

::

    !raid channel=worthing gym=Marine Gardens Restaurant boss=wailmer

Show all raids
--------------

This is to allow you to see all the raids that you have set up and this
is your reference for the raid id (left most column)

::

    !raid show

Returns:

::

    RAID ID |CHANNEL  |AREA/GYM     |BOSS/EGG   |LEVEL |MUTED
    --------+---------+-------------+-----------+------+-----
    32      |Sussex   |-            |All Eggs   |5     |     
    63      |Sussex   |-            |All Bosses |5     |     
    1       |Worthing |All          |All Eggs   |4     |     
    66      |Worthing |Ilex Way Park|All Eggs   |5     |     
    28      |Worthing |All          |All Bosses |4     |     
    34      |Worthing |All          |Machamp    |-     | 

There are a few extra options for this command (always in ascending
order)

::

    !raid show             Returns a list sorted Channel, Boss
    !raid show boss        Returns a list sorted by Boss, Channel
    !raid show channel     Returns a list sorted by Channel, Boss

Remove raid from table
----------------------

Remove by ID
~~~~~~~~~~~~

First run show command and note the raid alert id for the record you
want to remove

::

    !raid show

Returns:

::

    RAID ID |CHANNEL  |AREA    |BOSS/EGG   |LEVEL |MUTED
    --------+---------+--------+-----------+------+-----
    32      |Sussex   |-       |All Eggs   |5     |MUTED    
    66      |Worthing |Ferring |All Eggs   |5     |     

Once you have the raid alert id, you need to enter it in the mute
commands as below

::

    !raid remove 32        ------ 28 being the number in the Alert ID for the row to mute

RemoveAll alerts
~~~~~~~~~~~~~~~~

::

    !raid remove all       ------ This will mute all record for your user id

Remove by Location
~~~~~~~~~~~~~~~~~~

You can remove all alerts for a channel or an area within a channel:

::

    !raid remove channel="MidSussex"
    !raid remove channel="CentralEast" area="Covent Garden"

If removing an area, channel is still required.

Mute alert from table
---------------------

Mute by ID
~~~~~~~~~~

First run show command and note the raid alert id for the record you
want to mute

::

    !raid show

Returns:

::

    ID |POKEMON   |CHANNEL  |AREA            |IV  |CP   |MUTED  
    ---+----------+---------+----------------+----+-----|-----
    28 |Kadabra   |Brighton |All             |80  |1500 |

Once you have the raid alert id, you need to enter it in the mute
commands as below

::

    !raid mute 28        ------ 28 being the number in the raid alert ID for the row to mute

Mute All alerts
~~~~~~~~~~~~~~~

::

    !raid mute all       ------ This will mute all record for your user id

Mute by Location
~~~~~~~~~~~~~~~~

You can mute all raid alerts for a channel or an area within a channel:

::

    !raid mute channel="MidSussex"
    !raid mute channel="CentralEast" area="Covent Garden"

If muting an area, channel is still required.

Unmute raid from table
----------------------

Unmute by ID
~~~~~~~~~~~~

First run show command and note the raid alert id for the record you
want to mute

::

    !raid show

Returns:

::

    RAID ID |CHANNEL  |AREA    |BOSS/EGG   |LEVEL |MUTED
    --------+---------+--------+-----------+------+-----
    32      |Sussex   |-       |All Eggs   |5     |MUTED    
    66      |Worthing |Ferring |All Eggs   |5     |     

Once you have the raid alert id, you need to enter it in the mute
commands as below

::

    !raid unmute 32        ------ 28 being the number in the Alert ID for the row to mute

Unmute All alerts
~~~~~~~~~~~~~~~~~

::

    !raid unmute all       ------ This will mute all record for your user id

Unmute by Location
~~~~~~~~~~~~~~~~~~

You can unmute all alerts for a channel or an area within a channel:

::

    !raid unmute channel="MidSussex"
    !raid unmute channel="CentralEast" area="Covent Garden"

If unmuting an area, channel is still required.