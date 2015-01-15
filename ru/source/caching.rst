Кеширование
===========

Для кеширования Lynx использует сторонию библиотеку ovr\\cacher.

Как использовать
----------------

Перед тем как начать использовать кеширование вам нужно установить драйвер в класс ``Configuration`` и передать в ``EntityManager``.

Пример:

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

	use Cacher\Driver\Memcache;
	$configuration->setCacheDriver(new Memcache());

Memcached
---------

.. code-block:: php

	use Cacher\Driver\Memcached;
	$configuration->setCacheDriver(new Memcached());

Redis
---------

.. code-block:: php

	use Cacher\Driver\Redis;
	$configuration->setCacheDriver(new Redis());




