QueryBuilder
============

You can create new QueryBuilder:

.. code-block:: php
    $queryBuilder = $this->get('em')->createQueryBuilder();


Or create QueryBuilder from Repository object:

```
    $repository = $this->get('em')->getRepository('User');
    $userQueryBuilder = $repository->createQueryBuilder();
