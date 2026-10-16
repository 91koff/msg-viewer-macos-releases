# MSG Viewer for macOS

Бесплатный локальный просмотрщик файлов писем Microsoft Outlook (`.msg`).

**[Скачать последнюю версию / Download latest release](https://github.com/91koff/msg-viewer-macos-releases/releases/latest)**

## Установка и использование

1. Скачайте `MSG-Viewer-macOS.zip` в разделе Releases и распакуйте.
2. Перенесите **MSG Viewer.app** в папку **Программы** (или в `~/Applications`, если общая папка недоступна для записи).
3. Откройте приложение и выберите `.msg`. Несколько писем открываются в отдельных окнах.
4. Для открытия двойным щелчком: Finder → файл `.msg` → **Свойства** → **Открывать в программе** → **MSG Viewer** → **Изменить всё…**.

Требования: macOS 13 Ventura или новее; Apple Silicon или Intel. Apple Developer ID и нотариализация не используются: macOS может попросить разрешить первый запуск в **Конфиденциальность и безопасность**.

## Возможности

Текущий выпуск: **1.3.1 (16)**. Исправлены скачки окна при ручном изменении размера.

- Экспорт текущего письма в EML из верхней панели или меню «Файл» (**⇧⌘E**), с оформлением и доступными вложениями.
- Быстрый просмотр MSG в Finder по пробелу: поля письма, HTML и встроенные картинки.
- Три режима **HTML / TEXT / HEADERS**. HEADERS показывает исходные заголовки с копированием, поиском и масштабом; **⌥⌘U** включает этот режим.
- Перетаскивание одного или нескольких MSG на любую область окна со скруглённой подсветкой, в том числе поверх текста и вложений после изменения размера.
- Русский и английский интерфейс; по умолчанию язык macOS. Настройки: **⌘,**.
- Текст, HTML-оформление, таблицы и inline-картинки.
- Компактные поля отправителя, получателей, копии, темы и даты; вложения над текстом письма. Карточки переносятся в несколько рядов; встроенные картинки можно показать отдельным блоком кнопкой верхней панели.
- Цветные линии и вложенные отступы истории HTML-переписки; режим Text без цветных линий. Перенос длинных строк, ссылок и таблиц по ширине окна.
- Quick Look, открытие и сохранение вложений, просмотр вложенных писем.
- Поиск **⌘F**, масштаб **⌘+ / ⌘−**, сброс **⌘0**, несколько окон и сохранение масштаба.
- Автоматический размер для каждого письма, обычно до 30% ширины экрана, с минимумом под всю панель кнопок. Панель вмещается также при восстановлении размера и ручном сужении, включая запас под возврат и обновление. При выключенном автоматическом режиме ручной размер запоминается. Стартовое окно вмещает все три значка; версия приложения видна внизу. Настройки стали компактнее и открываются на мониторе окна письма.
- Системная, светлая и тёмная тема. Оригинальное оформление HTML-письма сохраняется.
- Проверка обновлений: при каждом запуске, раз в день, неделю или месяц; по умолчанию — неделя. В настройках «Проверить сейчас» меняется на «Обновить» при обнаружении новой версии.
- Значок обновления справа вверху и кнопка «Обновить» в настройках сразу запускают загрузку, проверку подписи, установку и перезапуск с восстановлением открытых писем.

Письма и вложения не отправляются на серверы. Интернет нужен только для обновлений. Исходные MSG не изменяются. Картинки из интернета и скрипты письма отключены. Для отображения картинки без интернета она должна быть сохранена внутри MSG.

Ограничения: MSG до 256 МБ; без PST/OST, расшифровки защищённых писем и OLE-объектов. При сохранении вложенного письма используется EML. Для неизвестного формата вложения потребуется соответствующее приложение Mac. Intel-сборка создана, но физический Intel Mac не использовался для проверки.

## Updates and installation (English)

Download and unzip `MSG-Viewer-macOS.zip`, then move **MSG Viewer.app** to Applications. Requires macOS 13+ on Apple Silicon or Intel. The app is locally signed, without Apple Developer ID notarization; macOS may require allowing the first launch in Privacy & Security.

To open `.msg` files by double-click: Finder → Get Info → Open with → MSG Viewer → Change All. Multiple messages open in separate windows.

Current release: **1.3.1 (16)**. Fixes window jumping during manual resizing. Settings (**⌘,**) include Russian/English/system language, appearance, per-message automatic sizing, a separate inline-image section and update frequency. Turn automatic sizing off to remember manual sizes. Compact Settings follow the message window’s display. The startup window fits all three toolbar buttons, and the app version appears at the bottom. Updates are checked only at launch, weekly by default, with every-launch/daily/monthly options. In Settings, Check now changes to Update when a newer version is found. The update badge at the top right and the Update button immediately start download, installation and restart, without an extra confirmation. Signed updates are verified before replacing the app; the previous version is restored if activation fails. Open messages are reopened after a successful update.

Export the current message as EML from the toolbar or File menu (**⇧⌘E**). Preview MSG in Finder with the Space bar. Switch **HTML / TEXT / HEADERS**; **⌥⌘U** shows the original headers with copy, find and zoom. The minimum message-window width fits every toolbar action, including Back and Update, even when restoring or resizing.

Drag one or more MSG files onto the window; a rounded highlight marks the drop area. Supports formatted HTML, tables, inline images, attachments, embedded messages, Quick Look, find (**⌘F**), zoom and **⌘0** to reset. Long lines and tables wrap to the window. HTML quote levels have colored bars; Text mode has none. Messages are processed locally and never uploaded. Remote images and message scripts are disabled. Maximum MSG size: 256 MB; encrypted messages, PST/OST and OLE objects are not supported.

## Release files

- `MSG-Viewer-macOS.zip`: universal macOS application.
- `SHA256SUMS`: archive checksum.
- `update.json` and `update.sig`: digitally signed update metadata used by the app.

This public repository contains ready-to-install binaries and user documentation. Source code is maintained separately in a private repository. No GitHub access token or private update-signing key is included in the application.
