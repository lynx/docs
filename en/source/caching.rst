Caching
=======

Lynx support many cache adapter from Cache sublib.

How to use
----------

Before starting to use caching driver you need to setup it in ``Configuration`` Class and pass it to Cache Manager

Example:

.. code-block:: php

	use Lynx\ORM\Configuration;
	use Lynx\Cache\NativeArray;

	$configuration = new Configuration();
	$configuration->setCacheDriver(new NativeArray());
