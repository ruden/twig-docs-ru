# Русская документация по шаблонизатору Twig

Оригинальную английскую документацию можно прочесть на сайте [twig.symfony.com](https://twig.symfony.com) или [GitHub](https://github.com/twigphp/Twig).

## Краткое содержание

* [О Twig](about.rst)
* [Введение / Установка](doc/intro.rst)
* [Twig для дизайнеров шаблонов](doc/templates.rst)
* [Twig для разработчиков](doc/api.rst)
* [Расширения Twig](doc/advanced.rst)
* [Twig Внутри](doc/internals.rst)
* [Twig Рецепты](doc/recipes.rst)
* [Стандарты кодирования](doc/coding_standards.rst)
* [License](https://twig.symfony.com/license)
 
### Быстрые ссылки

Просмотрите ссылки, чтобы узнать больше о встроенных функциях.

#### Теги

[apply](doc/tags/apply.rst),
[autoescape](doc/tags/autoescape.rst),
[block](doc/tags/block.rst),
[cache](doc/tags/cache.rst),
[deprecated](doc/tags/deprecated.rst),
[do](doc/tags/do.rst),
[embed](doc/tags/embed.rst),
[extends](doc/tags/extends.rst),
[filter](doc/tags/filter.rst),
[flush](doc/tags/flush.rst),
[for](doc/tags/for.rst),
[from](doc/tags/from.rst),
[if](doc/tags/if.rst),
[import](doc/tags/import.rst),
[include](doc/tags/include.rst),
[macro](doc/tags/macro.rst),
[sandbox](doc/tags/sandbox.rst),
[set](doc/tags/set.rst),
[spaceless](doc/tags/spaceless.rst),
[use](doc/tags/use.rst),
[verbatim](doc/tags/verbatim.rst)
[with](doc/tags/with.rst)

#### Фильтры

[abs](doc/filters/abs.rst),
[batch](doc/filters/batch.rst),
[capitalize](doc/filters/capitalize.rst),
[column](doc/filters/column.rst),
[convert_encoding](doc/filters/convert_encoding.rst),
[country_name](doc/filters/country_name.rst),
[currency_name](doc/filters/currency_name.rst),
[currency_symbol](doc/filters/currency_symbol.rst),
[data_uri](doc/filters/data_uri.rst),
[date](doc/filters/date.rst),
[date_modify](doc/filters/date_modify.rst),
[default](doc/filters/default.rst),
[escape](doc/filters/escape.rst),
[filter](doc/filters/filter.rst),
[first](doc/filters/first.rst),
[format](doc/filters/format.rst),
[format_currency](doc/filters/format_currency.rst),
[format_date](doc/filters/format_date.rst),
[format_datetime](doc/filters/format_datetime.rst),
[format_number](doc/filters/format_number.rst),
[format_time](doc/filters/format_time.rst),
[html_to_markdown](doc/filters/html_to_markdown.rst),
[inky_to_html](doc/filters/inky_to_html.rst),
[inline_css](doc/filters/inline_css.rst),
[join](doc/filters/join.rst),
[json_encode](doc/filters/json_encode.rst),
[keys](doc/filters/keys.rst),
[language_name](doc/filters/language_name.rst),
[last](doc/filters/last.rst),
[length](doc/filters/length.rst),
[lower](doc/filters/lower.rst),
[map](doc/filters/map.rst),
[markdown_to_html](doc/filters/markdown_to_html.rst),
[merge](doc/filters/merge.rst),
[nl2br](doc/filters/nl2br.rst),
[number_format](doc/filters/number_format.rst),
[raw](doc/filters/raw.rst),
[reduce](doc/filters/reduce.rst),
[replace](doc/filters/replace.rst),
[reverse](doc/filters/reverse.rst),
[round](doc/filters/round.rst),
[slice](doc/filters/slice.rst),
[slug](doc/filters/slug.rst),
[sort](doc/filters/sort.rst),
[spaceless](doc/filters/spaceless.rst),
[split](doc/filters/split.rst),
[striptags](doc/filters/striptags.rst),
[timezone_name](doc/filters/timezone_name.rst),
[title](doc/filters/title.rst),
[trim](doc/filters/trim.rst),
[upper](doc/filters/upper.rst),
[u](doc/filters/u.rst),
[url_encode](doc/filters/url_encode.rst)

#### Функции

[attribute](doc/functions/attribute.rst),
[block](doc/functions/block.rst),
[constant](doc/functions/constant.rst),
[country_timezones](doc/functions/country_timezones.rst),
[cycle](doc/functions/cycle.rst),
[date](doc/functions/date.rst),
[dump](doc/functions/dump.rst),
[html_classes](doc/functions/html_classes.rst),
[include](doc/functions/include.rst),
[max](doc/functions/max.rst),
[min](doc/functions/min.rst),
[parent](doc/functions/parent.rst),
[random](doc/functions/random.rst),
[range](doc/functions/range.rst),
[source](doc/functions/source.rst)
[template_from_string](doc/functions/template_from_string.rst)

#### Тесты

[constant](doc/tests/constant.rst),
[defined](doc/tests/defined.rst),
[divisibleby](doc/tests/divisibleby.rst),
[empty](doc/tests/empty.rst),
[even](doc/tests/even.rst),
[iterable](doc/tests/iterable.rst),
[null](doc/tests/null.rst),
[odd](doc/tests/odd.rst),
[sameas](doc/tests/sameas.rst)

#### Операторы

* [in](doc/templates.rst#containment-operator)
* [is](doc/templates.rst#test-operator)
* [Математические](doc/templates.rst#math) (+, -, /, %, //, *, **)
* [Логические](doc/templates.rst#math) (and, or, not, (), b-and, b-xor, b-or)
* [Сравнения](doc/templates.rst#comparisons) (==, !=, \<, \>, \>=, \<=, [===](doc/tests/sameas.rst))
* [Другие ](doc/templates.rst#other-operators) (.., \|, ~, ., [], ?:, ??)