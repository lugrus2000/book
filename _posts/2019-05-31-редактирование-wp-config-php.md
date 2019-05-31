---
ID: 31
post_title: >
  Редактирование
  wp-config.php
post_name: '%d1%80%d0%b5%d0%b4%d0%b0%d0%ba%d1%82%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-wp-config-php'
author: admin
post_date: 2019-05-31 09:38:49
layout: post
link: 'http://lugrus.ml/wp/%d1%80%d0%b5%d0%b4%d0%b0%d0%ba%d1%82%d0%b8%d1%80%d0%be%d0%b2%d0%b0%d0%bd%d0%b8%d0%b5-wp-config-php.html'
published: true
tags: [ ]
categories:
  - wordpress
---
<pre class='wp-markup-collection'>
## Редактирование wp-config.php

## Contents

- [1 Настройка базы данных](https://codex.wordpress.org/%D0%A0%D0%B5%D0%B4%D0%B0%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_wp-config.php#.D0.9D.D0.B0.D1.81.D1.82.D1.80.D0.BE.D0.B9.D0.BA.D0.B0_.D0.B1.D0.B0.D0.B7.D1.8B_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85)
- [1.1 Исходный wp-config-sample.php](https://codex.wordpress.org/%D0%A0%D0%B5%D0%B4%D0%B0%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_wp-config.php#.D0.98.D1.81.D1.85.D0.BE.D0.B4.D0.BD.D1.8B.D0.B9_wp-config-sample.php)
- [1.1.1 Укажите имя базы данных](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A3.D0.BA.D0.B0.D0.B6.D0.B8.D1.82.D0.B5_.D0.B8.D0.BC.D1.8F_.D0.B1.D0.B0.D0.B7.D1.8B_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85)
- [1.1.2 Укажите имя пользователя базы данных](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A3.D0.BA.D0.B0.D0.B6.D0.B8.D1.82.D0.B5_.D0.B8.D0.BC.D1.8F_.D0.BF.D0.BE.D0.BB.D1.8C.D0.B7.D0.BE.D0.B2.D0.B0.D1.82.D0.B5.D0.BB.D1.8F_.D0.B1.D0.B0.D0.B7.D1.8B_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85)
- [1.1.3 Укажите пароль к базе данных](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A3.D0.BA.D0.B0.D0.B6.D0.B8.D1.82.D0.B5_.D0.BF.D0.B0.D1.80.D0.BE.D0.BB.D1.8C_.D0.BA_.D0.B1.D0.B0.D0.B7.D0.B5_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85)
- [1.1.4 Укажите сервер базы данных](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A3.D0.BA.D0.B0.D0.B6.D0.B8.D1.82.D0.B5_.D1.81.D0.B5.D1.80.D0.B2.D0.B5.D1.80_.D0.B1.D0.B0.D0.B7.D1.8B_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85)
- [1.2 Возможные значения DB_HOST](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.92.D0.BE.D0.B7.D0.BC.D0.BE.D0.B6.D0.BD.D1.8B.D0.B5_.D0.B7.D0.BD.D0.B0.D1.87.D0.B5.D0.BD.D0.B8.D1.8F_DB_HOST)
- [1.3 Альтернативный порт MySQL](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.90.D0.BB.D1.8C.D1.82.D0.B5.D1.80.D0.BD.D0.B0.D1.82.D0.B8.D0.B2.D0.BD.D1.8B.D0.B9_.D0.BF.D0.BE.D1.80.D1.82_MySQL)
- [1.4 Кодировка базы данных](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9A.D0.BE.D0.B4.D0.B8.D1.80.D0.BE.D0.B2.D0.BA.D0.B0_.D0.B1.D0.B0.D0.B7.D1.8B_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85)
- [1.5 База данных параметр Сравнение](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.91.D0.B0.D0.B7.D0.B0_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85_.D0.BF.D0.B0.D1.80.D0.B0.D0.BC.D0.B5.D1.82.D1.80_.D0.A1.D1.80.D0.B0.D0.B2.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5)
- [1.6 Ключи безопасности](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9A.D0.BB.D1.8E.D1.87.D0.B8_.D0.B1.D0.B5.D0.B7.D0.BE.D0.BF.D0.B0.D1.81.D0.BD.D0.BE.D1.81.D1.82.D0.B8)
- [2 Расширенные опции](https://codex.wordpress.org/%D0%A0%D0%B5%D0%B4%D0%B0%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_wp-config.php#.D0.A0.D0.B0.D1.81.D1.88.D0.B8.D1.80.D0.B5.D0.BD.D0.BD.D1.8B.D0.B5_.D0.BE.D0.BF.D1.86.D0.B8.D0.B8)
- [2.1 префикс_таблиц](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.BF.D1.80.D0.B5.D1.84.D0.B8.D0.BA.D1.81_.D1.82.D0.B0.D0.B1.D0.BB.D0.B8.D1.86)
- [2.2 Адрес WordPress (URL)](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.90.D0.B4.D1.80.D0.B5.D1.81_WordPress_.28URL.29)
- [2.3 Адрес блога (URL)](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.90.D0.B4.D1.80.D0.B5.D1.81_.D0.B1.D0.BB.D0.BE.D0.B3.D0.B0_.28URL.29)
- [2.4 Перемещение wp-content](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9F.D0.B5.D1.80.D0.B5.D0.BC.D0.B5.D1.89.D0.B5.D0.BD.D0.B8.D0.B5_wp-content)
- [2.5 Перемещение папки загрузок](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9F.D0.B5.D1.80.D0.B5.D0.BC.D0.B5.D1.89.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.B0.D0.BF.D0.BA.D0.B8_.D0.B7.D0.B0.D0.B3.D1.80.D1.83.D0.B7.D0.BE.D0.BA)
- [2.6 Изменение интервала автосохранения](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.98.D0.B7.D0.BC.D0.B5.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B8.D0.BD.D1.82.D0.B5.D1.80.D0.B2.D0.B0.D0.BB.D0.B0_.D0.B0.D0.B2.D1.82.D0.BE.D1.81.D0.BE.D1.85.D1.80.D0.B0.D0.BD.D0.B5.D0.BD.D0.B8.D1.8F)
- [2.7 Редакции записей](https://codex.wordpress.org/%D0%A0%D0%B5%D0%B4%D0%B0%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_wp-config.php#.D0.A0.D0.B5.D0.B4.D0.B0.D0.BA.D1.86.D0.B8.D0.B8_.D0.B7.D0.B0.D0.BF.D0.B8.D1.81.D0.B5.D0.B9)
- [2.7.1 Отключить редакции записей](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9E.D1.82.D0.BA.D0.BB.D1.8E.D1.87.D0.B8.D1.82.D1.8C_.D1.80.D0.B5.D0.B4.D0.B0.D0.BA.D1.86.D0.B8.D0.B8_.D0.B7.D0.B0.D0.BF.D0.B8.D1.81.D0.B5.D0.B9)
- [2.7.2 Указать число редакций записи](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A3.D0.BA.D0.B0.D0.B7.D0.B0.D1.82.D1.8C_.D1.87.D0.B8.D1.81.D0.BB.D0.BE_.D1.80.D0.B5.D0.B4.D0.B0.D0.BA.D1.86.D0.B8.D0.B9_.D0.B7.D0.B0.D0.BF.D0.B8.D1.81.D0.B8)
- [2.8 Установить Cookie домен](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A3.D1.81.D1.82.D0.B0.D0.BD.D0.BE.D0.B2.D0.B8.D1.82.D1.8C_Cookie_.D0.B4.D0.BE.D0.BC.D0.B5.D0.BD)
- [2.9 Отладка](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9E.D1.82.D0.BB.D0.B0.D0.B4.D0.BA.D0.B0)
- [2.10 Отключить Javascript присоединение](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9E.D1.82.D0.BA.D0.BB.D1.8E.D1.87.D0.B8.D1.82.D1.8C_Javascript_.D0.BF.D1.80.D0.B8.D1.81.D0.BE.D0.B5.D0.B4.D0.B8.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5)
- [2.11 Настройка лога ошибок](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9D.D0.B0.D1.81.D1.82.D1.80.D0.BE.D0.B9.D0.BA.D0.B0_.D0.BB.D0.BE.D0.B3.D0.B0_.D0.BE.D1.88.D0.B8.D0.B1.D0.BE.D0.BA)
- [2.12 Увеличение памяти для PHP](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A3.D0.B2.D0.B5.D0.BB.D0.B8.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.B0.D0.BC.D1.8F.D1.82.D0.B8_.D0.B4.D0.BB.D1.8F_PHP)
- [2.13 КЭШ](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9A.D0.AD.D0.A8)
- [2.14 Пользовательские таблицы и Usermeta таблицы](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9F.D0.BE.D0.BB.D1.8C.D0.B7.D0.BE.D0.B2.D0.B0.D1.82.D0.B5.D0.BB.D1.8C.D1.81.D0.BA.D0.B8.D0.B5_.D1.82.D0.B0.D0.B1.D0.BB.D0.B8.D1.86.D1.8B_.D0.B8_Usermeta_.D1.82.D0.B0.D0.B1.D0.BB.D0.B8.D1.86.D1.8B)
- [2.15 Язык и Языковые Директории](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.AF.D0.B7.D1.8B.D0.BA_.D0.B8_.D0.AF.D0.B7.D1.8B.D0.BA.D0.BE.D0.B2.D1.8B.D0.B5_.D0.94.D0.B8.D1.80.D0.B5.D0.BA.D1.82.D0.BE.D1.80.D0.B8.D0.B8)
- [2.16 Сохранение запросов для анализа](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A1.D0.BE.D1.85.D1.80.D0.B0.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B7.D0.B0.D0.BF.D1.80.D0.BE.D1.81.D0.BE.D0.B2_.D0.B4.D0.BB.D1.8F_.D0.B0.D0.BD.D0.B0.D0.BB.D0.B8.D0.B7.D0.B0)
- [2.17 Смена прав доступа к файлам по умолчанию](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A1.D0.BC.D0.B5.D0.BD.D0.B0_.D0.BF.D1.80.D0.B0.D0.B2_.D0.B4.D0.BE.D1.81.D1.82.D1.83.D0.BF.D0.B0_.D0.BA_.D1.84.D0.B0.D0.B9.D0.BB.D0.B0.D0.BC_.D0.BF.D0.BE_.D1.83.D0.BC.D0.BE.D0.BB.D1.87.D0.B0.D0.BD.D0.B8.D1.8E)
- [2.18 Константы для обновления WordPress](https://codex.wordpress.org/%D0%A0%D0%B5%D0%B4%D0%B0%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_wp-config.php#.D0.9A.D0.BE.D0.BD.D1.81.D1.82.D0.B0.D0.BD.D1.82.D1.8B_.D0.B4.D0.BB.D1.8F_.D0.BE.D0.B1.D0.BD.D0.BE.D0.B2.D0.BB.D0.B5.D0.BD.D0.B8.D1.8F_WordPress)
- [2.18.1 Включение SSH Обновление доступа](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.92.D0.BA.D0.BB.D1.8E.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_SSH_.D0.9E.D0.B1.D0.BD.D0.BE.D0.B2.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B4.D0.BE.D1.81.D1.82.D1.83.D0.BF.D0.B0)
- [2.19 Альтернатива Cron](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.90.D0.BB.D1.8C.D1.82.D0.B5.D1.80.D0.BD.D0.B0.D1.82.D0.B8.D0.B2.D0.B0_Cron)
- [2.20 Дополнительно задаваемые константы](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.94.D0.BE.D0.BF.D0.BE.D0.BB.D0.BD.D0.B8.D1.82.D0.B5.D0.BB.D1.8C.D0.BD.D0.BE_.D0.B7.D0.B0.D0.B4.D0.B0.D0.B2.D0.B0.D0.B5.D0.BC.D1.8B.D0.B5_.D0.BA.D0.BE.D0.BD.D1.81.D1.82.D0.B0.D0.BD.D1.82.D1.8B)
- [2.21 Очистка корзины](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9E.D1.87.D0.B8.D1.81.D1.82.D0.BA.D0.B0_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD.D1.8B)
- [2.22 Автоматическая оптимизация базы данных](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.90.D0.B2.D1.82.D0.BE.D0.BC.D0.B0.D1.82.D0.B8.D1.87.D0.B5.D1.81.D0.BA.D0.B0.D1.8F_.D0.BE.D0.BF.D1.82.D0.B8.D0.BC.D0.B8.D0.B7.D0.B0.D1.86.D0.B8.D1.8F_.D0.B1.D0.B0.D0.B7.D1.8B_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85)
- [2.23 Просмотр всех определенных констант](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9F.D1.80.D0.BE.D1.81.D0.BC.D0.BE.D1.82.D1.80_.D0.B2.D1.81.D0.B5.D1.85_.D0.BE.D0.BF.D1.80.D0.B5.D0.B4.D0.B5.D0.BB.D0.B5.D0.BD.D0.BD.D1.8B.D1.85_.D0.BA.D0.BE.D0.BD.D1.81.D1.82.D0.B0.D0.BD.D1.82)
- [3 Дважды проверьте перед сохранением](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.94.D0.B2.D0.B0.D0.B6.D0.B4.D1.8B_.D0.BF.D1.80.D0.BE.D0.B2.D0.B5.D1.80.D1.8C.D1.82.D0.B5_.D0.BF.D0.B5.D1.80.D0.B5.D0.B4_.D1.81.D0.BE.D1.85.D1.80.D0.B0.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5.D0.BC)
- [4 Смотрите так же](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.A1.D0.BC.D0.BE.D1.82.D1.80.D0.B8.D1.82.D0.B5_.D1.82.D0.B0.D0.BA_.D0.B6.D0.B5)

Одним из шагов при установке WordPress является внесение в файл `wp-config.php` параметров, необходимых для доступа к базе данных MySQL.

Этот файл, `wp-config.php`, не содержится в скачиваемой копии WordPress; вам потребуется его создать. В качестве примера можно использовать файл `wp-config-sample.php`. Ниже представлены расширенные настройки и примеры.

Для изменения файла `wp-config.php` вам потребуется следующая информация:

- **Имя базы данных**

Имя базы данных для WordPress

- **Имя пользователя базы данных**

Имя пользователя для доступа к базе данных

- **Пароль к базе данных**

Пароль пользователя для доступа к базе данных

- **Сервер базы данных**

Имя сервера базы данных

Если WordPress установлен вашим хостинг-провайдером, узнайте эту информацию в службе поддержки. Если у вас свой собственный [сервер](https://codex.wordpress.org/Глоссарий#.D0.92.D0.B5.D0.B1-.D1.81.D0.B5.D1.80.D0.B2.D0.B5.D1.80) или хостинг, вы получите эту информацию в результате [создания базы данных и пользователя](https://codex.wordpress.org/Установка_WordPress#.D0.A8.D0.B0.D0.B3_2:_.D0.A1.D0.BE.D0.B7.D0.B4.D0.B0.D0.BD.D0.B8.D0.B5_.D0.B1.D0.B0.D0.B7.D1.8B_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85_.D0.B8_.D0.BF.D0.BE.D0.BB.D1.8C.D0.B7.D0.BE.D0.B2.D0.B0.D1.82.D0.B5.D0.BB.D1.8F).

## Настройка базы данных

**Важно:** *никогда* не используйте текстовые редакторы вроде Microsoft Word для изменения файлов WordPress!

Найдите в корневом каталоге WordPress файл `wp-config-sample.php` и откройте его в [текстовом редакторе](https://codex.wordpress.org/Глоссарий#.D0.A2.D0.B5.D0.BA.D1.81.D1.82.D0.BE.D0.B2.D1.8B.D0.B9_.D1.80.D0.B5.D0.B4.D0.B0.D0.BA.D1.82.D0.BE.D1.80).

**ЗАМЕЧАНИЕ:** Начиная с [версии 2.6](https://codex.wordpress.org/Version_2.6), [`wp-config.php` можно переместить](https://codex.wordpress.org/Редактирование_wp-config.php#.D0.9F.D0.B5.D1.80.D0.B5.D0.BC.D0.B5.D1.89.D0.B5.D0.BD.D0.B8.D0.B5_wp-content) в директорию на уровень выше той, в которой расположен WordPress.

### `Исходный wp-config-sample.php`

Это пример исходного файла `wp-config-sample.php`. Значения приведены здесь в качестве **примеров**. Изменения нужно вносить **не** здесь, а на своём сайте. Если вы с помощью кнопки «Править» внесёте изменения здесь, они **не** подействуют, а вы сообщите свой пароль всему миру.

[php]
// Параметры MySQL: Эту информацию можно получить у вашего хостинг-провайдера **

// Имя базы данных для WordPress

define('DB_NAME', '**putyourdbnamehere'**);

// Имя пользователя MySQL

define('DB_USER', '**usernamehere'**);

// Пароль к базе данных MySQL

define('DB_PASSWORD', '**yourpasswordhere'**);

// Имя сервера MySQL

define('DB_HOST', '**localhost'**);

[/php]

**ЗАМЕЧАНИЕ:** Текст внутри символов `/* */` — это комментарии, приведённые в справочных целях.

**ЗАМЕЧАНИЕ:** Не меняйте значения на этой странице, меняйте их на своём сервере.

#### Укажите имя базы данных

Замените `putyourdbnamehere` на имя вашей базы данных, например *МояБазаДанных*.

[php]
define('DB_NAME', 'МояБазаДанных'); // Пример имени базы данных
[/php]

#### Укажите имя пользователя базы данных

Замените `usernamehere` на имя вашего пользователя, например *МоёИмяПользователя*.

[php]
define('DB_USER', 'МоёИмяПользователя'); // Пример имени пользователя MySQL
[/php]

#### Укажите пароль к базе данных

Замените `yourpasswordhere` на ваш пароль, например *МойПароль*.

[php]
define('DB_PASSWORD', 'МойПароль'); // Пример пароля к MySQL
[/php]

#### Укажите сервер базы данных

Замените `localhost` на имя вашего сервера базы данных, например, *МойСерверБазыДанных*.

[php]
define('DB_HOST', 'МойСерверБазыДанных'); // Пример сервера базы данных MySQL
[/php]

**ЗАМЕЧАНИЕ:** Скорее всего, последнее значение менять **НЕ** придётся. Если вы не уверены, попробуйте установить WordPress со стандартным значением `'localhost'` в качестве имени сервера. Если установка завершится неудачей, обратитесь в службу поддержки вашего хостинг-провайдера.

### Возможные значения DB_HOST

Различные хостинг-провайдеры используют различные сетевые настройки для серверов MySQL. Если ваш хостинг-провайдер указан в левом столбце, соответствующее значение DB_HOST справа должно подойти. Для уверенности обратитесь в службу поддержки и/или посмотрите онлайн-документацию вашего хостинг-провайдера.

[bash]

| **Хостинг-провайдер** | **Вероятное значение DB_HOST** |
| -------------------------- | ----------------------------------------- |
| **1and1** | **db12345678** |
| **AN Hosting** | **localhost** |
| **A Small Orange** | **localhost** |
| **BlueHost** | **localhost** |
| **DreamHost** | **mysql.example.com** |
| **GoDaddy** | **h41mysql52.secureserver.net** |
| **HostGator** | **localhost** |
| **HostICan** | **localhost** |
| **ICDSoft** | **localhost:/tmp/mysql5.sock** |
| **LaughingSquid** | **localhost** |
| **MediaTemple GridServer** | **internal-db.s44441.gridserver.com** |
| **one.com** | **localhost** |
| **pair Networks** | **dbnnnx.pair.com** |
| **Rackspace Cloud** | **mysql50-01.wc1.dfw1.stabletransit.com** |
| **Yahoo** | **mysql** |
| **Сервера с cPanel** | **localhost** |
| **Сервера с Plesk** | **localhost** |
| **Сервера с DirectAdmin** | **localhost** |
| **Tophost.it** | **sql.your-domain-name.it** |
| **Sprinthost.ru** | **localhost** |

[/bash]

### Альтернативный порт MySQL

Если ваш хостинг-провайдер использует альтернативный порт для доступа к базе данных, нужно указать номер этого порта в параметре **DB_HOST** в файле `wp-config.php`.

Для localhost

[php]
define('DB_HOST', 'localhost:3307');
[/php]

Для другого сервера

[php]
define('DB_HOST', 'mysql.example.com:3307');
[/php]

Замените **3307** на номер порта, полученный от хостинг-провайдера.

### Кодировка базы данных

В WordPress [версии 2.2](https://codex.wordpress.org/Version_2.2) был введён параметр **DB_CHARSET**, чтобы иметь возможность указать [кодировку](https://codex.wordpress.org/Глоссарий#.D0.9A.D0.BE.D0.B4.D0.B8.D1.80.D0.BE.D0.B2.D0.BA.D0.B0) базы данных (например, tis620 для тайской кодировки TIS620) при работе с таблицами MySQL.

Стандартное значение **utf8** ([Unicode](http://en.wikipedia.org/wiki/Unicode) [UTF-8](http://en.wikipedia.org/wiki/UTF-8)) почти всегда является наилучшим вариантом. UTF-8 поддерживает все языки, поэтому в общем случае в качестве DB_CHARSET стоит оставить **utf8** и использовать значение [DB_COLLATE](https://codex.wordpress.org/Редактирование_wp-config.php#Database_collation) для вашего языка.

Этот пример показывает UTF 8, которая считается значением WordPress по умолчанию:

[php]
define('DB_CHARSET', 'utf8');
[/php]

**ВНИМАНИЕ:** Это применимо к новым инсталляциям

Там, как правило, не должно быть никаких причин для изменения значения DB_CHARSET по умолчанию. Если ваш блог нуждается в другом наборе символов, пожалуйста, прочитайте [поддерживаемые наборы символов и сопоставлений MySQL](http://dev.mysql.com/doc/refman/5.0/en/charset-charsets.html) для допустимых значений DB_CHARSET.

**ВНИМАНИЕ:** Это применимо к обновлениям (особенно блоги, которые существовали до версии 2.2)

Если DB_CHARSET и DB_COLLATE не присутствуют в вашем `wp-config.php` файле, **НЕ** добавляйте любого определения в ваш `wp-config.php` файл, если Вы не прочитали или не поняли [Преобразование базы данных наборов символов](https://codex.wordpress.org/Converting_Database_Character_Sets). Добавление DB_CHARSET и DB_COLLATE в файл `wp-config.php`, для существующего блога, может вызвать серьезные проблемы.

### База данных параметр Сравнение

As of WordPress [Version 2.2](https://codex.wordpress.org/Version_2.2), **DB_COLLATE** was made available to allow designation of the database [collation](https://codex.wordpress.org/Glossary#Collation) (i.e. the sort order of the character set). In most cases, this value should be left blank (null) so the database collation will be automatically assigned by MySQL based on the database character set specified by DB_CHARSET. Set **DB_COLLATE** to one of the UTF-8 values defined in [UTF-8 character sets](http://dev.mysql.com/doc/refman/5.0/en/charset-unicode-sets.html) для большинства западноевропейских языков.

The WordPress default DB_COLLATE value:

[php]
define('DB_COLLATE', );
[/php]

UTF-8 Unicode General collation

[php]
define('DB_COLLATE', 'utf8_general_ci');
[/php]

UTF-8 Unicode Turkish collation

[php]
define('DB_COLLATE', 'utf8_turkish_ci');
[/php]

**ВНИМАНИЕ:** Those performing new installations

There usually should be no reason to change the default value of DB_COLLATE. Leaving the value blank (null) will insure the collation is automatically assigned by MySQL when the database tables are created.

**ВНИМАНИЕ:** Those performing upgrades (especially blogs that existed before 2.2)

If DB_COLLATE and DB_CHARSET do not exist in your `wp-config.php` file, **DO NOT** add either definition to your `wp-config.php` file unless you read and understand [Converting Database Character Sets](https://codex.wordpress.org/Converting_Database_Character_Sets). And you may be in need of a WordPress upgrade.

### Ключи безопасности

In [Version 2.6](https://codex.wordpress.org/Version_2.6), three (3) security keys, **AUTH_KEY**, **SECURE_AUTH_KEY**, and **LOGGED_IN_KEY**, were added to insure better encryption of information stored in the user's cookies. (These collectively replaced a single key introduced in [Version 2.5](https://codex.wordpress.org/Version_2.5).) In [Version 2.7](https://codex.wordpress.org/Version_2.7) a fourth key, **NONCE_KEY**, was added to this group. When each key was added, corresponding salts were added: **AUTH_SALT**, **SECURE_AUTH_SALT**, **LOGGED_IN_SALT**, and **NONCE_SALT**.

You don't have to remember the keys, just make them long, random and complicated -- or better yet, use the [the online generator](https://api.wordpress.org/secret-key/1.1/salt/). You can change these at any point in time to invalidate all existing cookies. This does mean that all users will have to login again.

Пример (не используйте эти значения!):

[php]
define('AUTH_KEY', 't`DK%X:&amp;gt;xy|e-Z(BXb/f(Ur`8#~UzUQG-^_Cs_GHs5U-&amp;amp;Wb?pgn^p8(2@}IcnCa|');
define('SECURE_AUTH_KEY', 'D&amp;amp;ovlU#|CvJ##uNq}bel+^MFtT&amp;amp;.b9{UvR]g%ixsXhGlRJ7q!h}XWdEC[BOKXssj');
define('LOGGED_IN_KEY', 'MGKi8Br(&amp;amp;{H*~&amp;amp;0s;{k0&amp;lt;S(O:+f#WM+q|npJ-+P;RDKT:~jrmgj#/-,[hOBk!ry^');
define('NONCE_KEY', 'FIsAsXJKL5ZlQo)iD-pt??eUbdc{_Cn&amp;lt;4!d~yqz))&amp;amp;B D?AwK%)+)F2aNwI|siOe');
define('AUTH_SALT', '7T-!^i!0,w)L#JK@pc2{8XE[DenYI^BVf{L:jvF,hf}zBf883td6D;Vcy8,S)-&amp;amp;G');
define('SECURE_AUTH_SALT', 'I6`V|mDZq21-J|ihb u^q0F }F_NUcy`l,=obGtq*p#Ybe4a31R,r=|n#=]@]c #');
define('LOGGED_IN_SALT', 'w&amp;lt;$4c$Hmd%/*]`Oom&amp;gt;(hdXW|0M=X={we6;Mpvtg+V.o&amp;lt;$|#_}qG(GaVDEsn,~*4i');
define('NONCE_SALT', 'a|#h{c5|P &amp;amp;xWs4IZ20c2&amp;amp;%4!c(/uG}W:mAvy&amp;lt;I44`jAbup]t=]V&amp;lt;`}.py(wTP%%');
[/php]

A **secret key** makes your site harder to hack and access harder to crack by adding random elements to the password.

In simple terms, a secret key is a password with elements that make it harder to generate enough options to break through your security barriers. A password like &quot;password&quot; or &quot;test&quot; is simple and easily broken. A random, unpredictable password such as &quot;88a7da62429ba6ad3cb3c76a09641fc&quot; takes years to come up with the right combination. A '*salt* is used to further enhance the security of the generated result.

The four keys are required for the enhanced security. The four salts are recommended, but are not required, because WordPress will generate salts for you if none are provided. They are included in wp-config.php by default for inclusiveness.

For more information on the technical background and breakdown of secret keys and secure passwords, see:

[bash]

- [Ryan Boren - SSL and Cookies in WordPress 2.6](http://boren.nu/archives/2008/07/14/ssl-and-cookies-in-wordpress-26/)
- [WordPress Support Forum - HOWTO: Set up secret keys in WordPress 2.6+](http://wordpress.org/support/topic/170987)
- [Wikipedia's explanation of Password Cracking](http://en.wikipedia.org/wiki/Password_cracking)
- [Lorelle VanFossen - Protect Your Blog With a Solid Password](http://www.blogherald.com/2007/05/08/protect-your-blog-with-a-solid-password/)
- [Yahoo's Security Password Tips](http://security.yahoo.com/article.html?aid=2006102509)
- [Yahoo Security - How to Choose a Password](http://uk.security.yahoo.com/protect-your-privacy/choose-password.html)

[/bash]

&lt;h2&gt;Расширенные опции&lt;/h2&gt;
The following sections may contain advanced / unsupported information, so please make sure you practice [regular backups](https://codex.wordpress.org/WordPress_Backups) and know how to restore them before experimenting on a production installation.

### префикс_таблиц

The **$table_prefix** is the value placed in the front of your database tables. Change the value if you want to use something other than **wp_** for your database prefix. Typically this is changed if you are [installing multiple WordPress blogs](https://codex.wordpress.org/Installing_Multiple_Blogs) in the same database.

[php]
// You can have multiple installations in one database if you give each a unique prefix
$table_prefix = 'r235_'; // Only numbers, letters, and underscores please!
[/php]

A second blog installation using the same database can be achieved simply by using a different prefix than your other installations.

[php]
$table_prefix = 'y77_'; // Only numbers, letters, and underscores please!
[/php]

### Адрес WordPress (URL)

**WP_SITEURL**, defined since WordPress [Version 2.2](https://codex.wordpress.org/Version_2.2), allows the WordPress address (URL) to be defined. The valued defined is the address where your WordPress core files reside. It should include the http:// part too. Do not put a slash &quot;**/**&quot; at the end. Setting this value in `wp-config.php` overrides the [wp_options table](https://codex.wordpress.org/Database_Description#Table:_wp_options) value for **siteurl** and disables the WordPress address (URL) field in the [Administration](https://codex.wordpress.org/Administration_Panels) &amp;gt; [Settings](https://codex.wordpress.org/Administration_Panels#General) &amp;gt; [General](https://codex.wordpress.org/Settings_General_SubPanel) panel.

**ЗАМЕЧАНИЕ:** It won't change the Database value though, and the url will revert to the old database value if this line is removed from wp-config. [Use the **RELOCATE** constant](https://codex.wordpress.org/Changing_The_Site_URL#Relocate_method) to change the siteurl value in the database.

If WordPress is installed into a directory called &quot;wordpress&quot; for the [domain](http://en.wikipedia.org/wiki/Domain_name_system) example.com, define WP_SITEURL like this:

[php]
define('WP_SITEURL', 'http://example.com/wordpress');
[/php]

Dynamically set WP_SITEURL based on $_SERVER['HTTP_HOST']

[php]
define('WP_SITEURL', 'http://' . $_SERVER['HTTP_HOST'] . '/path/to/wordpressp');
[/php]

**ЗАМЕЧАНИЕ:** A safer alternative for some installations would be to use the server-generated SERVER_NAME instead of the php/user-generated HTTP_HOST which is created dynamically by php based on the value of the HTTP HOST Header in the request, thus possibly allowing for file inclusion vulnerabilities. SERVER_NAME is set by the server configuration and is static.

Dynamically set WP_SITEURL based on $_SERVER['SERVER_NAME']

[php]
define('WP_SITEURL', 'http://' . $_SERVER['SERVER_NAME'] . '/path/to/wordpressp');
[/php]

### Адрес блога (URL)

**WP_HOME** is another `wp-config.php` option added in WordPress [Version 2.2](https://codex.wordpress.org/Version_2.2). Similar to WP_SITEURL, WP_HOME *overrides the wp_options table value for* home *but does not change it permanently.* **home** is the address you want people to type in their browser to reach your WordPress blog. It should include the http:// part and should not have a slash &quot;**/**&quot; at the end.

[php]
define('WP_HOME', 'http://example.com/wordpress');
[/php]

If you are using the technique described in [Giving WordPress Its Own Directory](https://codex.wordpress.org/Giving_WordPress_Its_Own_Directory) then follow the example below. Remember, you will also be placing an `index.php` in your web-root directory if you use a setting like this.

[php]
define('WP_HOME', 'http://example.com');
[/php]

Dynamically set WP_HOME based on $_SERVER['HTTP_HOST']

[php]
define('WP_HOME', 'http://' . $_SERVER['HTTP_HOST'] . '/path/to/wordpress');
[/php]

### Перемещение wp-content

Since [Version 2.6](https://codex.wordpress.org/Version_2.6), you can move the `wp-content` directory, which holds your themes, plugins, and uploads, outside of the WordPress application directory.

Set WP_CONTENT_DIR to the full **local path** of this directory (no trailing slash), e.g.

[php]
define( 'WP_CONTENT_DIR', $_SERVER['DOCUMENT_ROOT'] . '/blog/wp-content' );
[/php]

Set WP_CONTENT_URL to the full **URI** of this directory (no trailing slash), e.g.

[php]
define( 'WP_CONTENT_URL', 'http://example/blog/wp-content');
[/php]

*Optional*
Set WP_PLUGIN_DIR to the full **local path** of this directory (no trailing slash), e.g.

[php]
define( 'WP_PLUGIN_DIR', $_SERVER['DOCUMENT_ROOT'] . '/blog/wp-content/plugins' );
[/php]

Set WP_PLUGIN_URL to the full **URI** of this directory (no trailing slash), e.g.

[php]
define( 'WP_PLUGIN_URL', 'http://example/blog/wp-content/plugins');
[/php]

If you have compability issues with plugins Set PLUGINDIR to the full **local path** of this directory (no trailing slash), e.g.

[php]
define( 'PLUGINDIR', $_SERVER['DOCUMENT_ROOT'] . '/blog/wp-content/plugins' );
[/php]

### Перемещение папки загрузок

Установить (к примеру) папку для загрузки медиафайлов на media:

[php]
define( 'UPLOADS', 'wp-content/media' );
[/php]

Этот путь не может быть абсолютным, он всегда относителен ABSPATH, поэтому не нужно указывать слеш в начале. Константа должна быть определена до этой директивы:

[php]
/** Sets up WordPress vars and included files. */
require_once(ABSPATH . 'wp-settings.php');
[/php]

### Изменение интервала автосохранения

При редактировании статьи, WordPress использует Ajax для автоматического сохранения изменений к статье при редактировании. Вы можете увеличить этот параметр для более длительной задержки между автоматическим сохранением, или уменьшить параметр, чтобы быть уверенным, что вы никогда не потеряете изменения. По умолчанию 60 секунд.

[php]
define('AUTOSAVE_INTERVAL', 160 ); // seconds
[/php]

### Редакции записей

WordPress по умолчанию, будет сохранять копии каждого редактирования сделанного к статье или странице, допуская возможность возврата к предыдущей версии этой статьи или страницы. Сохранение редакций может быть отключено, или максимальное количество редакций в статье или странице может быть указано.

#### Отключить редакции записей

Если вы **не** установите это значение, WordPress по-умолчанию присвоит `WP_POST_REVISIONS` в *true* (включены редакции статей). Если вы хотите отключить потрясающее свойство редакций, используйте этот параметр:

[php]
define('WP_POST_REVISIONS', false );
[/php]

#### Указать число редакций записи

Если вы хотите задать максимальное количество редакций, измените *false* на целое/число (*например*, `3` или `5`).

[php]
define('WP_POST_REVISIONS', 3);
[/php]

### Установить Cookie домен

Установка домена в cookies для WordPress может быть определена для тех, кто с необычными настройками домена. Одна из причин это если [субдомены используются для обслуживания статического контента](http://www.askapache.com/htaccess/apache-speed-subdomains.html). Для предотвращения отправки WordPress куков с каждым запросом к статическому контенту на вашем субдомене, вы можете установить куки только к вашему не-статическому домену.

[php]
define('COOKIE_DOMAIN', 'www.askapache.com');
[/php]

### Отладка

Опция `WP_DEBUG`, добавлена в WordPress [Version 2.3.1](https://codex.wordpress.org/Version_2.3.1), управляет отображением некоторых ошибок и предупреждений. Если этот параметр отсутствует в `wp-config.php`, то значение считается false.

**ЗАМЕЧАНИЕ:** Параметры *true* и *false* в примере не заключайте в апостроф (') , потому что они являются логическими значениями.

[php]
define('WP_DEBUG', true);
define('WP_DEBUG', false);
[/php]

Кроме того, если вы планируете модифицировать некоторые встроенные в WordPress JavaScript`ы, следует включить следующую опцию:

[php]
define('SCRIPT_DEBUG', true);
[/php]

Это позволит вам редактировать `*имя_скрипта*.dev.js` файлы в `wp-includes/js` и `wp-admin/js` каталогах.

[В WordPress начиная с версии 2.3.2, ошибки базы данных печатаются только если WP_DEBUG установлен в положение *true*](http://trac.wordpress.org/ticket/5473). В более ранних версиях, ошибки базы данных всегда печатались. (Ошибки базы данных обрабатываются классом wpdb и не влияют на [настройки ошибок РНР](http://www.php.net/errorfunc).)

В WordPress версии 2.5, установка WP_DEBUG в true также поднимает [уровень сообщений об ошибках](http://www.php.net/error-reporting) на E_ALL и активирует предупреждения, когда устаревшие функции или файлы используются; в противном случае, WordPress устанавливает уровень сообщений об ошибках в `E_ALL ^ E_NOTICE ^ E_USER_NOTICE`.

### Отключить Javascript присоединение

Чтобы результатам заканчиваться более быстрой административной областью, все файлы Javascript являются [присоединёнными](http://en.wikipedia.org/wiki/Concatenation) в один URL. Если Javascript не в состоянии работать в вашей административной области, вы можете попробовать отключить эту функцию:

[php]
define('CONCATENATE_SCRIPTS', false);
[/php]

### Настройка лога ошибок

Because `wp-config.php` is loaded for every page view not loaded from a cache file, it is an excellent location to set php ini settings that control your php installation. This is useful if you don't have access to a php.ini file, or if you just want to change some settings on the fly.

Here is an example that turns php error_logging on and logs them to a specific file. If `WP_DEBUG` is defined to true, the errors will also be saved to this file. Just place this above any *require_once* or *include* commands.

[php]
@ini_set('log_errors','On');
@ini_set('display_errors','Off');
@ini_set('error_log','/home/example.com/logs/php_error.log');
/* That's all, stop editing! Happy blogging. */
[/php]

Another example of logging errors, as suggested by Mike Little on the [wp-hackers email list](http://lists.automattic.com/pipermail/wp-hackers/2010-September/034830.html):

[php]
/**
* This will log all errors notices and warnings to a file called debug.log in
* wp-content (if Apache does not have write permission, you may need to create
* the file first and set the appropriate permissions (i.e. use 666) )
*/
define('WP_DEBUG', true);
define('WP_DEBUG_LOG', true);
define('WP_DEBUG_DISPLAY', false);
@ini_set('display_errors',0);
[/php]

### Увеличение памяти для PHP

Also released with [Version 2.5](https://codex.wordpress.org/Version_2.5), the **WP_MEMORY_LIMIT** option allows you to specify the maximum amount of memory that can be consumed by PHP. This setting may be necessary in the event you receive a message such as &quot;Allowed memory size of xxxxxx bytes exhausted&quot;.

This setting increases PHP Memory only for WordPress, not other applications. By default, WordPress will attempt to increase memory allocated to PHP to 32MB (code is at beginning of *wp-settings.php*), so the setting in *wp-config.php* should reflect something higher than 32MB.

WordPress will automatically check if PHP has been allocated less memory than the entered value before utilizing this function. For example, if PHP has been allocated 64MB, there is no need to set this value to 64M as WordPress will automatically use all 64MB if need be.

Пожалуйста, обратите внимание, что этот параметр не может работать, если ваш хостинг не позволяет увеличить объем памяти PHP - в этом случае , обратитесь к хостинг провайдеру для увеличение лимита PHP памяти. Кроме того, обратите внимание, что многие хостинги устанавливают лимит для PHP на 8 МБ.

Увеличить PHP память до 64 МБ

[php]
define('WP_MEMORY_LIMIT', '64M');
[/php]

Увеличить PHP память до 96 МБ

[php]
define('WP_MEMORY_LIMIT', '96M');
[/php]

### КЭШ

The **WP_CACHE** setting, if true, includes the `wp-content/advanced-cache.php` script, when executing `wp-settings.php`.

[php]
define('WP_CACHE', true);
[/php]

### Пользовательские таблицы и Usermeta таблицы

**CUSTOM_USER_TABLE** and **CUSTOM_USER_META_TABLE** are used to designated that the user and usermeta tables normally utilized by WordPress are not used, instead these values/tables are used to store your user information.

[php]
define('CUSTOM_USER_TABLE', $table_prefix.'my_users');
define('CUSTOM_USER_META_TABLE', $table_prefix.'my_usermeta');
[/php]

### Язык и Языковые Директории

**WPLANG** defines the name of the language translation (.mo) file. **WP_LANG_DIR** defines what directory the WPLANG .mo file resides. If WP_LANG_DIR is not defined WordPress looks first to wp-content/languages and then wp-includes/languages for the .mo defined by WPLANG file.

[php]
define ('WPLANG', 'ru_RU');
define('WP_LANG_DIR', $_SERVER['DOCUMENT_ROOT'].'wordpress/languages');
[/php]

### Сохранение запросов для анализа

The **SAVEQUERIES** definition saves the database queries to a array and that array can be displayed to help analyze those queries. The information saves each query, what function called it, and how long that query took to execute.

**NOTE:** This will have a performance impact on your site, so make sure to turn this off when you aren't debugging.

First, put this in wp-config.php:

[php]
define('SAVEQUERIES', true);
[/php]

Then in the footer of your theme put this:

[php]
&amp;lt;?php
if (current_user_can('administrator')){
global $wpdb;
echo &amp;quot;&amp;lt;pre&amp;gt;&amp;quot;;
print_r($wpdb-&amp;gt;queries);
echo &amp;quot;&amp;lt;/pre&amp;gt;&amp;quot;;
}
?&amp;gt;
[/php]

### Смена прав доступа к файлам по умолчанию

Команды **FS_CHMOD_DIR** и **FS_CHMOD_FILE** позволяют сменить права доступа к файлам и каталогам непосредственно из файла конфигурации. Это нужно, если возникает Ошибка 400. Такое может произойти на некоторых хостингах. Первая команда установит права доступа к каталогам на '**0755'** Вторая установит права доступа к файлам на '**0644'**. Не забудьте знак ('). Еще информация: [Changing File Permissions](https://codex.wordpress.org/Changing_File_Permissions)

[php]
define('FS_CHMOD_DIR', (0755 &amp;amp; ~ umask()));
define('FS_CHMOD_FILE', (0644 &amp;amp; ~ umask()));
[/php]

### Константы для обновления WordPress

**You should define as few of the below constants** needed to correct your update issues.

The most common causes of needing to define these are:

- Host running with a special installation setup involving Symlinks, You may need to define the path-related constants (FTP_BASE, FTP_CONTENT_DIR, and FTP_PLUGIN_DIR), Often defining simply the base will be enough.
- Certain PHP installations shiped with a PHP FTP Extension which is incompatible with certain FTP Servers, under these rare situations, you may need to define FTP_METHOD to 'ftpsockets'

The following are valid constants for WordPress updates:

- FS_METHOD

forces the filesystem method. It should only be &quot;direct&quot;, &quot;ssh&quot;, &quot;ftpext&quot;, or &quot;ftpsockets&quot;. Generally, You should only change this if you are experiencing update problems, If you change it, and it doesnt help

change it back/remove it

, Under most circumstances, setting it to 'ftpsockets' will work if the automatically chosen method does not.

- **(Primary Preference) &quot;Direct&quot;** forces it to use Direct File I/O requests from within PHP, this is fraught with opening up security issues on poorly configured hosts, This is chosen automatically when appropriate.
- **(Secondary Preference) &quot;ssh&quot;** is to force the usage of the SSH PHP Extension.
- **(3rd Preference) &quot;ftpext&quot;** is to force the usage of the FTP PHP Extension for FTP Access, and finally
- **(4th Preference) &quot;ftpsockets&quot;** utilises the PHP Sockets Class for FTP Access.

- **FTP_BASE** is the full path to the &quot;base&quot;(ABSPATH) folder of the WordPress installation.

- **FTP_CONTENT_DIR** is the full path to the wp-content folder of the WordPress installation.

- **FTP_PLUGIN_DIR** is the full path to the plugins folder of the WordPress installation.

- **FTP_PUBKEY** is the full path to your SSH public key.

- **FTP_PRIKEY** is the full path to your SSH private key.

- **FTP_USER** is either user FTP or SSH username. Most likely these are the same, but use the appropriate one for the type of update you wish to do.

- **FTP_PASS** is the password for the username entered for **FTP_USER**. If you are using SSH public key authentication this can be omitted.

- **FTP_HOST** is the hostname:port combination for your SSH/FTP server. The default FTP port is 21 and the default SSH port is 22, These do not need to be mentioned.

- **FTP_SSL** TRUE for SSL-connection *if supported by the underlying transport*, Not available on all servers. This is for &quot;Secure FTP&quot; not for SSH SFTP.

[php]
define('FS_METHOD', 'ftpext');
define('FTP_BASE', '/path/to/wordpress/');
define('FTP_CONTENT_DIR', '/path/to/wordpress/wp-content/');
define('FTP_PLUGIN_DIR ', '/path/to/wordpress/wp-content/plugins/');
define('FTP_PUBKEY', '/home/username/.ssh/id_rsa.pub');
define('FTP_PRIKEY', '/home/username/.ssh/id_rsa');
define('FTP_USER', 'username');
define('FTP_PASS', 'password');
define('FTP_HOST', 'ftp.example.org');
define('FTP_SSL', false);
[/php]

#### Включение SSH Обновление доступа

To enable SSH2 as an upgrade option you will need to install the pecl SSH2 extension. To install this library you will need to issue a command similar to the following or talk to your web hosting provider to get this installed:

[bash]
pecl install ssh2
[/bash]

After installing the pecl ssh2 extension you will need to modify your php configuration to automatically load this extension.

pecl is provided by the pear package in most linux distributions. To install pecl in Redhat/Fedora/CentOS:

[bash]
yum -y install php-pear
[/bash]

To install pecl in Debian/Ubuntu:

[bash]
apt-get install php-pear
[/bash]

It is recommended to use a private key that is not pass-phrase protected. There have been numerous reports that pass phrase protected private keys do not work properly. If you decide to try a pass phrase protected private key you will need to enter the pass phrase for the private key as FTP_PASS, or entering it in the &quot;Password&quot; field in the presented credential field when installing updates.

If you're still not clear on how to use SSH for upgrading or installing WordPress/plugins, [read through this tutorial](http://www.firesidemedia.net/dev/wordpress-install-upgrade-ssh/).

### Альтернатива Cron

Use this, for example, if scheduled posts are not getting published. According to [Otto's forum explanation](http://wordpress.org/support/topic/296236?replies=13#post-1175405), &quot;this alternate method uses a redirection approach, which makes the users browser get a redirect when the cron needs to run, so that they come back to the site immediately while cron continues to run in the connection they just dropped. This method is a bit iffy sometimes, which is why it's not the default.&quot;

[php]
define('ALTERNATE_WP_CRON', true);
[/php]

### Дополнительно задаваемые константы

Here are additional constants that can be defined, but probably shouldn't be. The Cookie definitions are particularly useful if you have an unusual domain setup.

[php]
define('COOKIEPATH', preg_replace('|https?://[^/]+|i', '', get_option('home') . '/' ) );
define('SITECOOKIEPATH', preg_replace('|https?://[^/]+|i', '', get_option('siteurl') . '/' ) );
define('ADMIN_COOKIE_PATH', SITECOOKIEPATH . 'wp-admin' );
define('PLUGINS_COOKIE_PATH', preg_replace('|https?://[^/]+|i', '', WP_PLUGIN_URL) );
define('TEMPLATEPATH', get_template_directory());
define('STYLESHEETPATH', get_stylesheet_directory());
define('DISABLE_WP_CRON', true);
[/php]

### Очистка корзины

Added with [Version 2.9](https://codex.wordpress.org/Version_2.9), this constant controls the number of days before WordPress permanently deletes posts, pages, attachments, and comments, from the trash bin. The default is 30 days:

[php]
define('EMPTY_TRASH_DAYS', 30 ); // 30 days
[/php]

To disable trash set the number of days to zero. Note that WordPress will not ask for confirmation when someone clicks on &quot;Delete Permanently&quot;.

[php]
define('EMPTY_TRASH_DAYS', 0 ); // zero days
[/php]

### Автоматическая оптимизация базы данных

Added with [Version 2.9](https://codex.wordpress.org/Version_2.9), there is automatic database optimization support, which you can enable by adding the following define to your wp-config.php file **only when the feature is required**

[php]
define('WP_ALLOW_REPAIR', true);
[/php]

The script can be found at `{$your_site}/wp-admin/maint/repair.php`

**Please Note:** That this define **enables** the functionality, **The user does not need to be logged in to access this functionality when this define is set.** This is because its main intent is to repair a corrupted database, Users can often not login when the database is corrupt.

### Просмотр всех определенных констант

Php has a function that returns an array of all the currently defined constants with their values.

[php]
print_r(@get_defined_constants());
[/php]

## Дважды проверьте перед сохранением

***Be sure to check for leading and/or trailing spaces around any of the above values you entered, and DON'T delete the single quotes!***

Before you save the file, be sure to **double-check** that you have not accidentally deleted any of the single quotes around the parameter values. Be sure there is nothing after the closing PHP tag in the file. The last thing in the file should be **?&amp;gt;** and nothing else. No spaces.

To save the file, choose **File &amp;gt; Save As &amp;gt; wp-config.php** and save the file in the root of your WordPress install. Upload the file to your web server and you're ready to install WordPress!

### Смотрите так же

- [WordPress Backups](https://codex.wordpress.org/WordPress_Backups)
- [Installing Multiple Blogs requires special wp-config.php](https://codex.wordpress.org/Installing_Multiple_Blogs)
- [Troubleshooting Installations](https://codex.wordpress.org/Upgrading_WordPress_Extended)
- [Securing your Installation](https://codex.wordpress.org/Administration_Over_SSL)

### Categories

- [ru:Getting Started](https://codex.wordpress.org/index.php?title=Category:ru:Getting_Started&amp;amp;action=edit&amp;amp;redlink=1)
- [ru:Advanced Topics](https://codex.wordpress.org/index.php?title=Category:ru:Advanced_Topics&amp;amp;action=edit&amp;amp;redlink=1)
- [ru:Installation](https://codex.wordpress.org/index.php?title=Category:ru:Installation&amp;amp;action=edit&amp;amp;redlink=1)
- [ru:UI Link](https://codex.wordpress.org/index.php?title=Category:ru:UI_Link&amp;amp;action=edit&amp;amp;redlink=1)
- [ru:Error Handling](https://codex.wordpress.org/index.php?title=Category:ru:Error_Handling&amp;amp;action=edit&amp;amp;redlink=1)
- [Russian Codex](https://codex.wordpress.org/Category:Russian_Codex)

[pmid-refs key= limit=5]
</pre>