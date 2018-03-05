***********
Subscribing
***********

.. contents:: :local:

Why Should I Subscribe?
#######################

There are many reasons why subscribing is possibly the best thing you could ever do :) Not only do you get the warm fuzzy feeling from knowing that your support is keeping this service running, 
but you also get ALL of the following goodies!!

* Access to the scan channels to see what is spawning in the areas you want to know about  
* Access to the map  
* Access to :doc:`Arceus </arceus/intro>`, our pokemon alert bot. This can be customised to alert you for pokemon based on location, IV, CP, Level and more.
* Access to :doc:`Dialga </dialga/intro>`, our raid alert bot. This can be customised to alert you to raids in your chosen area or at specific gyms.

Cost of Subscription
####################

The minimum subscription cost is £1, which will cover you for 10 days. This works out to 10p a day! 
You can subscribe for whatever length of time you want; there is no maximum subscription but we would advise against subscribing too far into the future, due to the nature of our service. 
Niantic could enforce changes that would result in the potential closure of our service without much notice, and refunds will not be processed should this happen.

.. warning::

	Guzzlord will only read whole pound amounts, so if you pay £2.50, your subscription will only be for 20 days, or £2 worth.

How To Subscribe
################

Make Payment
============ 

Make a payment via `PayPal <http://bit.ly/2igVOxV>`_. Make note of the transaction ID for the payment.

.. note::

	Payment can only be made in GBP, and must have a value of at least £1. Anything less will be rejected by Guzzlord. Also, payments cannot be processed until marked as 'Complete' in PayPal.

Apply Payment
=============

Go to the bot-commands channel and type:

.. code-block:: bash

    !subscribe
	
In DM with Guzzlord, type:
 
.. code-block:: bash

    !transction <ID>

where <ID> is the transaction ID you noted in step 1. If the transaction ID is correct and found on `PayPal <http://bit.ly/2igVOxV>`_, you will receive a response with your new subscription expiry date.

.. image:: subscribe_response.PNG

.. note::

	Please remember, if you are subscribing again after expiring, your map credentials will have changed. If extending your subscription, your credentials will remain unchanged.
 
Get Map Credentials
===================

Type:

.. code-block:: bash

    !map
	
In DM with Guzzlord to get the URL of the map, and your credentials for logging onto the map. If desired you can also change your password (see below)

Expiration
==========

You will be sent a reminder 3 days before your subscription expires and again once it does. Should your subscription expire, your map credentials will be deleted, your bot rights will be revoked
and you will no longer be able to see the scan channels. Your alerts will not be deleted until you leave the server in case you decide to re-subscribe.

Useful Commands 
###############

All commands must be done in DM with Guzzlord.

.. code-block:: bash

    !change_password newpassword
	
If you want to change your map password to something shorter or more memorable.

.. note::

    Passwords are stored in the DB as plain text. Please do not use a password that you use elsewhere.
	
.. code-block:: bash

    !expiry

If you want to check your expiry date, use this command. 

.. code-block:: bash

    !calculate amount

Want to find out how much bang for your buck you get? Use this command to work out the expiry date for a given amount, for example ``!calculate 5``