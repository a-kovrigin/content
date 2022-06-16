---
title: SA-CORE-2022-010
slug: wiki/security/sa-core-2022-010
metatags:
  title: 'Drupal: SA-CORE-2022-010'
  description: 'Умеренно критично. Исправлено в версиях: 9.3.14, 9.2.20.'
authors:
  - Niklan
---

**Проект:** Drupal Core\
**Дата публикации:** 25 мая 2022\
**Риск безопасности:** Умеренно критично 13∕25. AC:Basic/A:User/CI:Some/II:Some/E:Theoretical/TD:Default\
**Уязвимость:** Сторонние библиотеки

## Описание

Drupal использует стороннюю библиотеку Guzzle для управления запросами и ответами к сторонним сервисам. Guzzle выпустили обновление безопасности, которое не влияет на Drupal ядро, но может на некоторые сторонние модули или пользовательский код.

Данный релиз безопасности выпущен за пределами обычного расписания, поскольку Guzzle уже опубликовал информацию об уязвимости, и они могут существовать на проектах которые используют библиотеку для внешних запросов. Guzzle оценил данную уязвимость как «Высокий риск».

[Drupal Steward](https://www.drupal.org/steward) не покрывает данную проблему.

## Решение

Обновиться до актуальных версий:

- Если используете Drupal 9.3, обновитесь до Drupal [9.3.14](../../../releases/9/9.3.x/9.3.14/index.md).
- Если используете Drupal 9.2, обновитесь до Drupal [9.2.20](../../../releases/9/9.2.x/9.2.20/index.md).

## Ссылки

- [SA-CORE-2022-010](https://www.drupal.org/SA-CORE-2022-010) (англ.), drupal.org, 25 мая 2022
- [Cross-domain cookie leakage](https://github.com/guzzle/guzzle/security/advisories/GHSA-cwmx-hcrq-mhc3) (англ.), github.com, 25 мая 2022