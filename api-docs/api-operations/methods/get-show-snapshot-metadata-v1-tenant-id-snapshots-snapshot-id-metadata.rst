
.. _get-show-snapshot-metadata:

Show snapshot metadata
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code::

    GET /v1/{tenant_id}/snapshots/{snapshot_id}/metadata

This operation shows the metadata for the specified snapshot.



This table shows the possible response codes for this operation:


+--------------------------+-------------------------+-------------------------+
|Response Code             |Name                     |Description              |
+==========================+=========================+=========================+
|200                       |OK                       |Success                  |
+--------------------------+-------------------------+-------------------------+


Request
""""""""""""""""




This table shows the URI parameters for the request:

+--------------------------+-------------------------+-------------------------+
|Name                      |Type                     |Description              |
+==========================+=========================+=========================+
|{tenant_id}               |String *(Required)*      |The unique identifier of |
|                          |                         |the tenant or account.   |
+--------------------------+-------------------------+-------------------------+
|{snapshot_id}             |String *(Required)*      |The unique identifier of |
|                          |                         |an existing snapshot.    |
+--------------------------+-------------------------+-------------------------+





This operation does not accept a request body.




Response
""""""""""""""""










**Example: Show snapshot metadata JSON response**


.. code::

   
   
   {
       "snapshot": {
           "status": "available",
           "os-extended-snapshot-attributes:progress": "0%",
           "description": null,
           "created_at": "2014-05-06T17:59:52.000000",
           "metadata": {
               "key": "v1"
           },
           "volume_id": "ebd80b99-bc3d-4154-9d28-5583baa80580",
           "os-extended-snapshot-attributes:project_id": "7e0105e19cd2466193729ef78b604f79",
           "size": 10,
           "id": "dfcd17fe-3b64-44ba-b95f-1c9c7109ef95",
           "name": "my-snapshot"
       }
   }
   




