Caching
=======

For cache, we use another library - ovr/cacher.

How to use
----------

Before starting to use caching driver you need to setup it in ``Configuration`` Class and pass it to Cache Manager

Example:

.. code-block:: php

	use Lynx\ORM\Configuration;
	use Cacher\Driver\NativeArray;

	$configuration = new Configuration();
	$configuration->setCacheDriver(new NativeArray());

NativeArray
-----------

.. code-block:: php

	use Cacher\Driver\NativeArray;
	$configuration->setCacheDriver(new NativeArray());

Memcache
--------

.. code-block:: php

	use Cacher\Driver\NativeArray;
	$configuration->setCacheDriver(new Memcache());

Memcached
---------

.. code-block:: php

	use Cacher\Driver\NativeArray;
	$configuration->setCacheDriver(new Memcached());
	
Redis
---------

.. code-block:: php

	use Cacher\Driver\Redis;
	$configuration->setCacheDriver(new Redis());
