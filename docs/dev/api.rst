========================
RESTful API for CRAMS
========================

The data stored in CRAMS instances is made accessible through
a RESTful API.

The API version ``v1`` is built on the Tastypie framework ??

The RESTful API can also be explored via the automatically generated Swagger
documentation at  < location>

See `swagger.io`_ for details on the Swagger standard.

.. _`swagger.io`: http://swagger.io

API accessible models
=====================




Authentication
==============




  

Querying the database (GET)
===========================

All endpoints support querying lists and individual records via GET requests.
Some support more complex queries via GET parameters as well.


Creating objects, adding files (POST)
=====================================

The creation of Experiments, Datasets and Dataset_Files via POSTs with the
option to include metadata/parametersets has been implemented and tested.

The following examples demonstrate how to go about it.

In all except the file attachment case the POST data should be a JSON string,
the ``Content-Type`` header needs to be set to ``application/json`` and the
``Accept`` header as well. Other response formats may be made available in the
future.

In all cases the URI of the created object is returned in the ``Location``
header of the response.


Example JSON input


   

Example JSON input:




