``constant``
============

``constant`` проверяет, имеет ли переменная то же самое значение, что и константа. Вы
можете использовать либо глобальные константы или константы класса:

.. code-block:: twig

    {% if post.status is constant('Post::PUBLISHED') %}
        атрибут status в точности совпадает с атрибутом Post::PUBLISHED
    {% endif %}

Можно также проверить константы из экземпляров объекта:

.. code-block:: twig

    {% if post.status is constant('PUBLISHED', post) %}
        атрибут status в точности совпадает с атрибутом Post::PUBLISHED
    {% endif %}
