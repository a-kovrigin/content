---
title: SA-CORE-2021-008
slug: security/sa-core-2021-008
metatags:
  title: 'Drupal: SA-CORE-2021-008'
  description: 'Умеренно критично. Исправлено в версиях: 8.9.19, 9.1.13, 9.2.6.'
---

**Проект:** Drupal Core\
**Дата публикации:** 15 сентября 2021\
**Риск безопасности:** Умеренно критично. Critical 11∕25 AC:Basic/A:None/CI:None/II:Some/E:Theoretical/TD:Uncommon\
**Уязвимость:** Обход доступа

## Описание

Модули Drupal — JSON:API, File и REST позволяют загружать файлы с использованием их HTTP API. Модули делали не все проверки файлов корректно, что приводит к уязвимости обхода доступа. Злоумышленник может иметь возможность загружать файлы в обход процесса проверки файлов реализованных модулями на сайте.

Эту уязвимость представляет опасность в трёх случаях:

* Включён модуль JSON:API или REST загрузка файлов.
* Злоумышленник имеет права на загрузку файлов с использованием JSON:API или REST.
* На сайте используется модуль проверки файлов.

[Drupal Steward](https://www.drupal.org/steward) не покрывает данную проблему.

## Решение

Обновиться до актуальных версий:

- Если используете Drupal 9.2.x, обновитесь до [Drupal 9.2.6](../../../releases/9/9.2.x/9.2.6/index.md).
- Если используете Drupal 9.1.x, обновитесь до [Drupal 9.1.13](../../../releases/9/9.1.x/9.1.13/index.md).
- Если используете Drupal 8.9.x, обновитесь до [Drupal 8.9.19](../../../releases/8/8.9.x/8.9.19/index.md).

## Ссылки

- [SA-CORE-2021-008](https://www.drupal.org/sa-core-2021-008) (англ.), drupal.org, 15 сентября 2021