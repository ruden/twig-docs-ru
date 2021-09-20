<p align="center"><a href="https://paypal.me/ValeriiRudenko/10"><img src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" alt="paypal"></a></p>

О Twig
======

Twig это современный шаблонизатор для PHP
-----------------------------------------

* **Быстрый**: Twig  *компилирует*  шаблоны в оптимизированный PHP код. Использование памяти по сравнению с обычным PHP кодом сведено к минимуму.

* **Безопасный**: Twig имеет режим  "песочницы"  для оценки "ненадежного" кода в шаблонах. Это позволяет использовать Twig в приложениях, где пользователи могут менять содержимое шаблонов.

* **Гибкий**: Twig использует гибко настраиваемые  *лексический* и  *грамматический* анализаторы. Это позволяет разработчику определять свои теги и   фильтры, создавать собственный DSL.

Что делает Twig лучше PHP в качестве шаблонизатора?
---------------------------------------------------

Когда дело доходит до шаблонизаторов в PHP, многие люди скажут вам, что сам PHP является шаблонизатором. Но даже если PHP начал свою жизнь как язык шаблонов, он не развивался так, как в последние годы. На самом деле, он не поддерживает многие функции, которые должны иметь современные шаблонизаторы:

* **Краткость**:Язык PHP многословен и даже слишком многословен, когда надо экранировать вывод данных::

```php
    <?php echo $var ?>
    <?php echo htmlspecialchars($var, ENT_QUOTES, 'UTF-8') ?>
```

  Twig имеет более лаконичный синтаксис, который позволяет легко читать шаблоны:

```twig
    {{ var }}
    {{ var|escape }}
    {{ var|e }}         {# сокращение для escape #}
```

* **Ориентированный на шаблоны синтаксис**:Twig имеет сокращения для многих общих паттернов, например, отображение текста по умолчанию, если вы перебираете пустой массив:

```twig
    {% for user in users %}
        * {{ user.name }}
    {% else %}
        Пользователи не найдены.
    {% endfor %}
```

* **Полнофункциональный**:Twig поддерживает все, что вам надо для использования шаблонов: множественное наследование, блоки, автоматическое экранирование и многое другое:

```twig
    {% extends "layout.html" %}

    {% block content %}
        Содержимое страницы...
    {% endblock %}
```

* **Легок в изучении**:Синтаксис просто изучить и оптимален для верстальщиков, что позволяет им быстро выполнять свою работу.

Конечно, для PHP написано большое число шаблонизаторов. Но большинство из них написаны под PHP и не используют лучшие практики разработки:

* **Расширяемость**: Twig - гибкий движок для любых ваших потребностей, даже самых сложных. Благодаря открытой архитектуре, вы можете определять новые языковые конструкции (тэги и фильтры) для создания своего собственного DSL.

* **Юнит-тестирование**: Twig полностью покрыт тестами. Библиотека стабильна и готова к использованию в больших проектах.

* **Документация**: Twig полностью документирован, вся документация доступна на сайте, и, конечно, имеет полное описание API.

* **Безопасность**: В отношении безопасности, Twig имеет несколько совершенно уникальных особенностей:

  * *Автоматическое экранирование вывода*: Для безопасного вывода данных, вы можете включить экранирование как глобально, так и для отдельных блоков:

```twig
    {% autoescape on %}
    {% var %}
    {% var|safe %}     {# var не экранируется #}
    {% var|escape %}   {# var не экранируется дважды #}
    {% endautoescape %}
```

* *Песочница*: Twig позволяет использовать для любого шаблона "песочницу", где пользователи имеют ограниченный набор тэгов, фильтров и методов объектов, определенных разработчиком. Режим "песочницы" может быть включен как глобально, так и локально, для определенных шаблонов:

```twig
    {{ include "user.html" sandboxed }}
```

* **Чистые сообщения об ошибках**: Каждый раз, когда у вас возникают синтаксические ошибки в шаблоне, Twig выводит сообщение о имени файла с ошибкой и номере строки, которая ее вызвала. Это очень упрощает отладку.

* **Быстрый**: Одна из целей создания Twig - сделать его таким быстрым как только можно. Для достижения максимальной скорости работы, Twig компилирует шаблоны в оптимизированный PHP код. Использование памяти по сравнению с обычным PHP кодом сведено к минимуму.