Русская документация по шаблонизатору Twig
==========================================

Оригинальную английскую документацию можно прочесть на сайте `twig.symfony.com`_ или `GitHub`_.

Краткое содержание
------------------

* `О Twig </about.rst>`_
* `Введение / Установка </doc/intro.rst>`_
* `Twig для дизайнеров шаблонов </doc/templates.rst>`_
* `Twig для разработчиков </doc/api.rst>`_
* `Расширения Twig </doc/advanced.rst>`_
* `Twig Внутри </doc/internals.rst>`_
* `Twig Рецепты </doc/recipes.rst>`_
* `Стандарты кодирования </doc/coding_standards.rst>`_
* `License`_

Быстрые ссылки
~~~~~~~~~~~~~~

Просмотрите ссылку, чтобы узнать больше о встроенных функциях.

Теги
''''

`apply </doc/tags/apply.rst>`_,
`autoescape </doc/tags/autoescape.rst>`_,
`block </doc/tags/block.rst>`_,
`cache </doc/tags/cache.rst>`_,
`deprecated </doc/tags/deprecated.rst>`_,
`do </doc/tags/do.rst>`_,
`embed </doc/tags/embed.rst>`_,
`extends </doc/tags/extends.rst>`_,
`filter </doc/tags/filter.rst>`_,
`flush </doc/tags/flush.rst>`_,
`for </doc/tags/for.rst>`_,
`from </doc/tags/from.rst>`_,
`if </doc/tags/if.rst>`_,
`import </doc/tags/import.rst>`_,
`include </doc/tags/include.rst>`_,
`macro </doc/tags/macro.rst>`_,
`sandbox </doc/tags/sandbox.rst>`_,
`set </doc/tags/set.rst>`_,
`spaceless </doc/tags/spaceless.rst>`_,
`use </doc/tags/use.rst>`_,
`verbatim </doc/tags/verbatim.rst>`_
`with </doc/tags/with.rst>`_

Фильтры
'''''''

`abs </doc/filters/abs.rst>`_,
`batch </doc/filters/batch.rst>`_,
`capitalize </doc/filters/capitalize.rst>`_,
`column </doc/filters/column.rst>`_,
`convert_encoding </doc/filters/convert_encoding.rst>`_,
`country_name </doc/filters/country_name.rst>`_,
`currency_name </doc/filters/currency_name.rst>`_,
`currency_symbol </doc/filters/currency_symbol.rst>`_,
`data_uri </doc/filters/data_uri.rst>`_,
`date </doc/filters/date.rst>`_,
`date_modify </doc/filters/date_modify.rst>`_,
`default </doc/filters/default.rst>`_,
`escape </doc/filters/escape.rst>`_,
`filter </doc/filters/filter.rst>`_,
`first </doc/filters/first.rst>`_,
`format </doc/filters/format.rst>`_,
`format_currency </doc/filters/format_currency.rst>`_,
`format_date </doc/filters/format_date.rst>`_,
`format_datetime </doc/filters/format_datetime.rst>`_,
`format_number </doc/filters/format_number.rst>`_,
`format_time </doc/filters/format_time.rst>`_,
`html_to_markdown </doc/filters/html_to_markdown.rst>`_,
`inky_to_html </doc/filters/inky_to_html.rst>`_,
`inline_css </doc/filters/inline_css.rst>`_,
`join </doc/filters/join.rst>`_,
`json_encode </doc/filters/json_encode.rst>`_,
`keys </doc/filters/keys.rst>`_,
`language_name </doc/filters/language_name.rst>`_,
`last </doc/filters/last.rst>`_,
`length </doc/filters/length.rst>`_,
`lower </doc/filters/lower.rst>`_,
`map </doc/filters/map.rst>`_,
`markdown_to_html </doc/filters/markdown_to_html.rst>`_,
`merge </doc/filters/merge.rst>`_,
`nl2br </doc/filters/nl2br.rst>`_,
`number_format </doc/filters/number_format.rst>`_,
`raw </doc/filters/raw.rst>`_,
`reduce </doc/filters/reduce.rst>`_,
`replace </doc/filters/replace.rst>`_,
`reverse </doc/filters/reverse.rst>`_,
`round </doc/filters/round.rst>`_,
`slice </doc/filters/slice.rst>`_,
`slug </doc/filters/slug.rst>`_,
`sort </doc/filters/sort.rst>`_,
`spaceless </doc/filters/spaceless.rst>`_,
`split </doc/filters/split.rst>`_,
`striptags </doc/filters/striptags.rst>`_,
`timezone_name </doc/filters/timezone_name.rst>`_,
`title </doc/filters/title.rst>`_,
`trim </doc/filters/trim.rst>`_,
`upper </doc/filters/upper.rst>`_,
`u </doc/filters/u.rst>`_,
`url_encode </doc/filters/url_encode.rst>`_

Функции
'''''''

`attribute </doc/functions/attribute.rst>`_,
`block </doc/functions/block.rst>`_,
`constant </doc/functions/constant.rst>`_,
`country_timezones </doc/functions/country_timezones.rst>`_,
`cycle </doc/functions/cycle.rst>`_,
`date </doc/functions/date.rst>`_,
`dump </doc/functions/dump.rst>`_,
`html_classes </doc/functions/html_classes.rst>`_,
`include </doc/functions/include.rst>`_,
`max </doc/functions/max.rst>`_,
`min </doc/functions/min.rst>`_,
`parent </doc/functions/parent.rst>`_,
`random </doc/functions/random.rst>`_,
`range </doc/functions/range.rst>`_,
`source </doc/functions/source.rst>`_
`template_from_string </doc/functions/template_from_string.rst>`_

Тесты
'''''

`constant </doc/tests/constant.rst>`_,
`defined </doc/tests/defined.rst>`_,
`divisibleby </doc/tests/divisibleby.rst>`_,
`empty </doc/tests/empty.rst>`_,
`even </doc/tests/even.rst>`_,
`iterable </doc/tests/iterable.rst>`_,
`null </doc/tests/null.rst>`_,
`odd </doc/tests/odd.rst>`_,
`sameas </doc/tests/sameas.rst>`_

Операторы
'''''''''

* `in </doc/templates.rst#containment-operator>`_
* `is </doc/templates.rst#test-operator>`_
* `Математические </doc/templates.rst#math>`_ (+, -, /, %, //, *, **)
* `Логические </doc/templates.rst#math>`_ (and, or, not, (), b-and, b-xor, b-or)
* `Сравнения </doc/templates.rst#comparisons>`_ (==, !=, \<, \>, \>=, \<=, `=== </doc/tests/sameas.rst>`_)
* `Другие  </doc/templates.rst#other-operators>`_ (.., |, ~, ., [], ?:, ??)

.. _`GitHub`: https://github.com/twigphp/Twig
.. _`twig.symfony.com`: https://twig.symfony.com/
.. _`License`: https://twig.symfony.com/license
