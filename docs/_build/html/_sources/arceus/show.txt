***************************
Showing Alerts & Exclusions
***************************

## Contents:

- [Viewing Alerts] (#viewing-alerts)
- [Viewing Exclusions] (#viewing-exclusions)

## Viewing Filters

.. code-block:: bash

    !alert show

Shows a list of alerts. It’s the go-to to see what’s going on with filters. Example:

.. image:: alert_show.PNG
    :align: center

.. code-block:: bash

    !alert show name`  
    !alert show number`

Shows a list of filters, sorted by name or by (dex) number.

## Viewing Exclusions

If you alerts have exclusions, you can view these by typing:

.. code-block:: bash

    !exclude show <ID>
