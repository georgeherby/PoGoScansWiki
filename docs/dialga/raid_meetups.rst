************
Raid Meetups
************

.. contents:: :local:

Using dialga, you can create meetups for all raids that are level 4 or higher. Lower levels do not need this functionality as can be completed solo, or need at most 2 people. 
All the current raids that can have a meetup created can be found in the ``-activeraids channel``. This channel will show you all the current level 4+ raids, and also any meetups that have already been organised.

To attend or create meetups, commands must be posted in the ``-raidchat`` channel.

.. note::

	To create a meetup, you need the ID of the raid in the ``-activeraids`` channel. To attend a meetup, you need the ID of the meetup in the same channel.

Create a meetup
---------------

To create a meet-up type:

::

	!setup <raid_id> <meet time>  
	
For example ``!setup 32 18:00``

If you have are bringing extra people to the meet there is an additonal parameter you can add:

::

	!setup <raid_id> <meet time> <extra people>
	
For example ``!setup 32 21:00 3`` if bringing three extra people with you.

EX Raid
~~~~~~~

To create a meetup for an upcoming EX raid :

::

	!ex "<gym name>" <meetup day> <24hr_time>
	
For example ``!ex "St Mary's" 20/03/2018 17:00``

Attend a meetup
---------------

To attend a meet-up:

::

	!attend <raid_id>
	
For example ``!attend 32``

If you are bringing plus ones, add that number to the
end of the command, for example ``!attend 32 2``

Can No Longer Attend?
---------------------

If you have marked yourself as attending a meet-up but can no longer
attend, please type:

::

	!decline <raid_id> 
	
For example ``!decline 32``

.. note::

	If you were the only person attending the meetup, once you decline the meetup will be deleted.

Who is attending a meetup?
--------------------------

To see who is going to a meet-up, type:

::

	!who <raid_id>
	
for example ``!who 32``

Where is the Raid/Meetup?
-------------------------

Raid
~~~~

If you are unsure as to the location of a raid, type:

::

	!where-raid <raid_id>
	
For example ``!where-raid 32``

Meetup
~~~~~~

If you are unsure as to the location of a meetup, type

::

	!where-meetup <meetup_id> 
	
For example ``!where-meetup 32``