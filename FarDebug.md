# Описание #

> Плагин представляет собой frontend для windows-версии консольного отладчика GNU Debuger - gdb (http://www.gnu.org/software/gdb/), и позволяет отлаживать программы, скомпилированные любым компилятором, поддерживающим совместимый формат отладочной информации (gcc, g++, free pascal и др.). Возможна отладка как 32-х так и 64-х разрядных приложений (для отладки 64-х разрядных приложений требуется 64-х разрядная версия отладчика gdb64, но _не_ требуется Far64).

> Плагин предоставляет простой интерфейс к основным возможностям отладчика:
    * Пошаговая отладка, с использованием текстового редактора FAR
    * Просмотр переменных и вычисление выражений
    * Установка контрольных точек
    * Просмотр стека вызовов
    * Просмотр и отладка машинного кода

> Все возможности отладчика также доступны в командном режиме через окно "Debug console"

> [Примеры](FarDebug_Samples.md)

> Обсуждение:<br>
<blockquote><a href='http://forum.farmanager.com/viewtopic.php?f=5&t=4235'>http://forum.farmanager.com/viewtopic.php?f=5&amp;t=4235</a></blockquote>

<h2>Загрузить</h2>

<ul><li><a href='http://far-plugins.googlecode.com/files/FarDebug.v3.rar'>FarDebug 1.0.3 for FAR 2</a>
</li><li><a href='http://far-plugins.googlecode.com/files/FarDebug.x64.v3.rar'>FarDebug 1.0.3 for FAR 2 x64</a></li></ul>

<blockquote>GDB:</blockquote>

<ul><li><a href='http://sourceforge.net/projects/mingw/files/'>MinGW</a>
</li><li><a href='http://cygwin.com/install.html'>CygWin</a></li></ul>


<hr />

<h1>История изменений</h1>

<h2>Ver 1.0.3</h2>

<ul><li>Добавлено окно "Disassemble", с возможностью пошаговой отладки на уровне машинного кода (F2)</li></ul>

<ul><li>Добавлено окно помощи по командам GDB (Window->Help)</li></ul>

<ul><li>Для поддержки отладки DLL, в диалог "Open" добавлено поле ввода "Host Application"</li></ul>

<ul><li>В окне "Breakpoint" можно добавлять точки останова через диалог (Ins). Точки останова, добавленные из редактора попадают в единую историю.</li></ul>

<ul><li>Глобальный и локальные файлы пресетов (содержат команды, которые будут автоматически переданы отладчику)</li></ul>

<blockquote>Глобальный файл называется "presets.ini" и находится в каталоге плагина. Пресеты из этого файла исполняются один раз, при загрузки GDB.</blockquote>

<blockquote>Локальный файл называется FarDebug.ini и должен находится в каталоге отлаживаемого модуля. Пресеты из этого файла исполняются каждый раз после загрузки модуля, до начала отладки.</blockquote>

<ul><li>Добавлена команда "Leave" - исполнение до выхода из процедуры</li></ul>

<ul><li>Недоступные команды главного меню запрещаются.</li></ul>

<ul><li>Небольшое меню настроек</li></ul>

<ul><li>В комплект добавлен FML макрос для с основными командами отладки</li></ul>

<ul><li>Изменены алгоритмы взаимодействия с отладчиком GDB</li></ul>

<ul><li>Исправлено несколько ошибок.</li></ul>

<h2>Ver 1.0.2</h2>

<ul><li>В диалоге Sources List работает упорядочивание по имени файла (Ctrl-F1) или по пути (Ctrl-F2)</li></ul>

<ul><li>В диалоге выбора каталога исходных файлов добавлена кнопка "Обзор" (требуется наличие плагина DialogTools)</li></ul>

<ul><li>Исправлено несколько ошибок.</li></ul>

<h2>Ver 1.0.1</h2>

<ul><li>В главное меню добавлена команда "Find Address", позволяющая быстро перейти на исходный текст по адресу. Допустим ввод нескольких адресов через разделители.</li></ul>

<ul><li>Улучшено позиционирование в редакторе при трассировке и переходе из окон отладчика.</li></ul>

<ul><li>Исправлено несколько ошибок.