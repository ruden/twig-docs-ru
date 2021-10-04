# Русская документация по шаблонизатору Twig

Оригинальную английскую документацию можно прочесть на сайте [twig.symfony.com](https://twig.symfony.com) или [GitHub](https://github.com/twigphp/Twig).

## Краткое содержание

* [О Twig](about.rst)
* [Введение / Установка](intro.rst)
* [Twig для дизайнеров шаблонов](templates.rst)
* [Twig для разработчиков](api.rst)
* [Расширения Twig](advanced.rst)
* [Twig Внутри](internals.rst)
* [Twig Рецепты](recipes.rst)
* [Стандарты кодирования](coding_standards.rst)
* [License](https://twig.symfony.com/license)
 
## Быстрые ссылки

Просмотрите ссылки, чтобы узнать больше о встроенных функциях.

### Теги

[apply](tags/apply.rst),
[autoescape](tags/autoescape.rst),
[block](tags/block.rst),
[cache](tags/cache.rst),
[deprecated](tags/deprecated.rst),
[do](tags/do.rst),
[embed](tags/embed.rst),
[extends](tags/extends.rst),
[filter](tags/filter.rst),
[flush](tags/flush.rst),
[for](tags/for.rst),
[from](tags/from.rst),
[if](tags/if.rst),
[import](tags/import.rst),
[include](tags/include.rst),
[macro](tags/macro.rst),
[sandbox](tags/sandbox.rst),
[set](tags/set.rst),
[spaceless](tags/spaceless.rst),
[use](tags/use.rst),
[verbatim](tags/verbatim.rst)
[with](tags/with.rst)

### Фильтры

[abs](filters/abs.rst),
[batch](filters/batch.rst),
[capitalize](filters/capitalize.rst),
[column](filters/column.rst),
[convert_encoding](filters/convert_encoding.rst),
[country_name](filters/country_name.rst),
[currency_name](filters/currency_name.rst),
[currency_symbol](filters/currency_symbol.rst),
[data_uri](filters/data_uri.rst),
[date](filters/date.rst),
[date_modify](filters/date_modify.rst),
[default](filters/default.rst),
[escape](filters/escape.rst),
[filter](filters/filter.rst),
[first](filters/first.rst),
[format](filters/format.rst),
[format_currency](filters/format_currency.rst),
[format_date](filters/format_date.rst),
[format_datetime](filters/format_datetime.rst),
[format_number](filters/format_number.rst),
[format_time](filters/format_time.rst),
[html_to_markdown](filters/html_to_markdown.rst),
[inky_to_html](filters/inky_to_html.rst),
[inline_css](filters/inline_css.rst),
[join](filters/join.rst),
[json_encode](filters/json_encode.rst),
[keys](filters/keys.rst),
[language_name](filters/language_name.rst),
[last](filters/last.rst),
[length](filters/length.rst),
[lower](filters/lower.rst),
[map](filters/map.rst),
[markdown_to_html](filters/markdown_to_html.rst),
[merge](filters/merge.rst),
[nl2br](filters/nl2br.rst),
[number_format](filters/number_format.rst),
[raw](filters/raw.rst),
[reduce](filters/reduce.rst),
[replace](filters/replace.rst),
[reverse](filters/reverse.rst),
[round](filters/round.rst),
[slice](filters/slice.rst),
[slug](filters/slug.rst),
[sort](filters/sort.rst),
[spaceless](filters/spaceless.rst),
[split](filters/split.rst),
[striptags](filters/striptags.rst),
[timezone_name](filters/timezone_name.rst),
[title](filters/title.rst),
[trim](filters/trim.rst),
[upper](filters/upper.rst),
[u](filters/u.rst),
[url_encode](filters/url_encode.rst)

### Функции

[attribute](functions/attribute.rst),
[block](functions/block.rst),
[constant](functions/constant.rst),
[country_timezones](functions/country_timezones.rst),
[cycle](functions/cycle.rst),
[date](functions/date.rst),
[dump](functions/dump.rst),
[html_classes](functions/html_classes.rst),
[include](functions/include.rst),
[max](functions/max.rst),
[min](functions/min.rst),
[parent](functions/parent.rst),
[random](functions/random.rst),
[range](functions/range.rst),
[source](functions/source.rst)
[template_from_string](functions/template_from_string.rst)

### Тесты

[constant](tests/constant.rst),
[defined](tests/defined.rst),
[divisibleby](tests/divisibleby.rst),
[empty](tests/empty.rst),
[even](tests/even.rst),
[iterable](tests/iterable.rst),
[null](tests/null.rst),
[odd](tests/odd.rst),
[sameas](tests/sameas.rst)

### Операторы

* [in](templates.rst#containment-operator)
* [is](templates.rst#test-operator)
* [Математические](templates.rst#math) (+, -, /, %, //, *, **)
* [Логические](templates.rst#math) (and, or, not, (), b-and, b-xor, b-or)
* [Сравнения](templates.rst#comparisons) (==, !=, \<, \>, \>=, \<=, [===](tests/sameas.rst))
* [Другие](templates.rst#other-operators) (.., \|, ~, ., [], ?:, ??)

## Ссылки на Twig от Symfony

Symfony предоставляет гораздо больше возможностей ``symfony/twig-bridge`` через пакет Composer.

### Теги

[form_theme](https://twig.symfony.com/doc/3.x/tags/form_theme.html),
[stopwatch](https://twig.symfony.com/doc/3.x/tags/stopwatch.html),
[trans](https://twig.symfony.com/doc/3.x/tags/trans.html),
[trans_default_domain](https://twig.symfony.com/doc/3.x/tags/trans_default_domain.html),
[transchoice](https://twig.symfony.com/doc/3.x/tags/transchoice.html)

### Фильтры

[abbr_class](https://twig.symfony.com/doc/3.x/filters/abbr_class.html),
[abbr_method](https://twig.symfony.com/doc/3.x/filters/abbr_method.html),
[file_excerpt](https://twig.symfony.com/doc/3.x/filters/file_excerpt.html),
[file_link](https://twig.symfony.com/doc/3.x/filters/file_link.html),
[file_relative](https://twig.symfony.com/doc/3.x/filters/file_relative.html),
[format_args](https://twig.symfony.com/doc/3.x/filters/format_args.html),
[format_args_as_text](https://twig.symfony.com/doc/3.x/filters/format_args_as_text.html),
[format_file](https://twig.symfony.com/doc/3.x/filters/format_file.html),
[format_file_from_text](https://twig.symfony.com/doc/3.x/filters/format_file_from_text.html),
[humanize](https://twig.symfony.com/doc/3.x/filters/humanize.html),
[trans](https://twig.symfony.com/doc/3.x/filters/trans.html),
[transchoice](https://twig.symfony.com/doc/3.x/filters/transchoice.html),
[yaml_dump](https://twig.symfony.com/doc/3.x/filters/yaml_dump.html),
[yaml_encode](https://twig.symfony.com/doc/3.x/filters/yaml_encode.html)

### Функции

[absolute_url](https://twig.symfony.com/doc/3.x/functions/absolute_url.html),
[asset](https://twig.symfony.com/doc/3.x/functions/asset.html),
[asset_version](https://twig.symfony.com/doc/3.x/functions/asset_version.html),
[controller](https://twig.symfony.com/doc/3.x/functions/controller.html),
[csrf_token](https://twig.symfony.com/doc/3.x/functions/csrf_token.html),
[expression](https://twig.symfony.com/doc/3.x/functions/expression.html),
[form](https://twig.symfony.com/doc/3.x/functions/form.html),
[form_end](https://twig.symfony.com/doc/3.x/functions/form_end.html),
[form_errors](https://twig.symfony.com/doc/3.x/functions/form_errors.html),
[form_help](https://twig.symfony.com/doc/3.x/functions/form_help.html),
[form_label](https://twig.symfony.com/doc/3.x/functions/form_label.html),
[form_rest](https://twig.symfony.com/doc/3.x/functions/form_rest.html),
[form_row](https://twig.symfony.com/doc/3.x/functions/form_row.html),
[form_start](https://twig.symfony.com/doc/3.x/functions/form_start.html),
[form_widget](https://twig.symfony.com/doc/3.x/functions/form_widget.html),
[is_granted](https://twig.symfony.com/doc/3.x/functions/is_granted.html),
[logout_path](https://twig.symfony.com/doc/3.x/functions/logout_path.html),
[logout_url](https://twig.symfony.com/doc/3.x/functions/logout_url.html),
[path](https://twig.symfony.com/doc/3.x/functions/path.html),
[relative_path](https://twig.symfony.com/doc/3.x/functions/relative_path.html),
[render](https://twig.symfony.com/doc/3.x/functions/render.html),
[render_esi](https://twig.symfony.com/doc/3.x/functions/render_esi.html),
[url](https://twig.symfony.com/doc/3.x/functions/url.html)

### Тесты

[rootform](https://twig.symfony.com/doc/3.x/tests/rootform.html),
[selectedchoice](https://twig.symfony.com/doc/3.x/tests/selectedchoice.html)