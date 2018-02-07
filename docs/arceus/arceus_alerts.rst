Pokemon Alerts
==============

To receive DM alerts for Pokemon posted to discord, you need to set up
alerts using Arceus. There are two types of alert:

1. Channel/Area alerts
2. Location based alerts

Users in Sussex and Home Counties have the option of both types, but
London may only set up location based alerts.

To set up locations before proceeding to create alerts, click `here`_

NOTE: You can switch your alerts between location and channel/area based
very easily should you want. Instructions on how to do this are at the
end of the location wiki above.

**All commands should be run in DM (Direct Message) to Arceus**

[TOC]

Set alerts for Pokemon
----------------------

For this you must format your commands in one of the formats below.

**Trainer Tip - you can change the minimum IV/CP/Level of alerts after
using the command in** ##Change Minimum IV/CP for alerts

If you have issues with entering invalid channels go to #help and type
``!channels`` and this will give a list of available channels to enter
in the command

Single Channel alerts
~~~~~~~~~~~~~~~~~~~~~

So if you want examples of how to get alerts for Reading, Worthing or
Brighton for example see below.

No Minimum Filters
^^^^^^^^^^^^^^^^^^

``!alert pokemon=Unown channel=worthing area=all`` *using channel &
area* ``!alert pokemon=Unown`` *to use location*

Minimum IV & CP
^^^^^^^^^^^^^^^

``!alert pokemon=Ampharos channel=reading area=reading cp=2000 iv=100``
*using channel & area* ``!alert pokemon=Ampharos cp=2000 iv=100`` *to
use location*

Minimum IV & Level
^^^^^^^^^^^^^^^^^^

``!alert pokemon=Lapras channel=Brighton area=East Brighton iv=100 level=30``
*using channel & area* ``!alert pokemon=Lapras iv=100 level=30`` *to use
location*

Minimum CP & Level
^^^^^^^^^^^^^^^^^^

``!alert pokemon=Tyranitar channel=worthing area=durrington cp=2500 level=30``
*using channel & area* ``!alert pokemon=Tyranitar cp=2500 level=30`` *to
use location*

Minimum CP or Level or IV
^^^^^^^^^^^^^^^^^^^^^^^^^

``!alert pokemon=Snorlax channel=slough area=all cp=2500``
``!alert pokemon=Snorlax channel=slough area=all iv=95``
``!alert pokemon=Snorlax channel=slough area=all level=30`` *using
channel & area*

``!alert pokemon=Snorlax cp=2500`` ``!alert pokemon=Snorlax iv=95``
``!alert pokemon=Snorlax level=30`` *to use location*

Alerts for All Pokemon or All Pokemon by Generation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**you can only apply these alerts with a filter (IV/CP/Level)**

``!alert pokemon=All channel=Slough area=All cp=2500``
``!alert pokemon=All channel=Reading area=Caversham iv=95``
``!alert pokemon=All channel=MidSussex area=All level=30 iv=100``
``!alert pokemon=gen1 channel=Worthing area=All iv=90``
``!alert pokemon=gen3 channel=Eastbourne area=All iv=100 level=35``
*using channel & area*

``!alert pokemon=All cp=2500`` ``!alert pokemon=All iv=95``
``!alert pokemon=All level=30 iv=100`` ``!alert pokemon=gen1 iv=90``
``!alert pokemon=gen3 iv=100 level=35`` *to use location*

Excluding certain Pokemon from alerts
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

When using the multiple pokemon alert typ

.. _here: https://bitbucket.org/georgeherby/arceus/wiki/Location%20Commands
