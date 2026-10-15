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

- Перетаскивание одного или нескольких MSG на окно со скруглённой подсветкой области сброса.
- Русский и английский интерфейс; по умолчанию язык macOS. Настройки: **⌘,**.
- Текст, HTML-оформление, таблицы и inline-картинки.
- Поля отправителя, получателей, копии и даты; вложения над текстом письма.
- Quick Look, открытие и сохранение вложений, просмотр вложенных писем.
- Поиск **⌘F**, масштаб **⌘+ / ⌘−**, несколько окон и сохранение размера/масштаба.
- Системная, светлая и тёмная тема. Оригинальное оформление HTML-письма сохраняется.
- Проверка обновлений при запуске: день, неделя, месяц; по умолчанию — неделя. Ручная проверка в настройках.
- Значок обновления справа вверху запускает загрузку, проверку подписи, установку и перезапуск с восстановлением открытых писем.

Письма и вложения не отправляются на серверы. Интернет нужен только для обновлений. Исходные MSG не изменяются. Картинки из интернета и скрипты письма отключены. Для отображения картинки без интернета она должна быть сохранена внутри MSG.

Ограничения: MSG до 256 МБ; без PST/OST, расшифровки защищённых писем и OLE-объектов. При сохранении вложенного письма используется EML. Для неизвестного формата вложения потребуется соответствующее приложение Mac. Intel-сборка создана, но физический Intel Mac не использовался для проверки.

## Updates and installation (English)

Download and unzip `MSG-Viewer-macOS.zip`, then move **MSG Viewer.app** to Applications. Requires macOS 13+ on Apple Silicon or Intel. The app is locally signed, without Apple Developer ID notarization; macOS may require allowing the first launch in Privacy & Security.

To open `.msg` files by double-click: Finder → Get Info → Open with → MSG Viewer → Change All. Multiple messages open in separate windows.

Settings (**⌘,**) include Russian/English/system language, appearance and update frequency. Updates are checked only at launch, weekly by default, with daily/monthly options and a manual Check now button. An update badge at the top right starts download and installation. Signed updates are verified before replacing the app; the previous version is restored if activation fails. Open messages are reopened after a successful update.

Drag one or more MSG files onto the window; a rounded highlight marks the drop area. Supports formatted HTML, tables, inline images, attachments, embedded messages, Quick Look, find (**⌘F**) and zoom. Messages are processed locally and never uploaded. Remote images and message scripts are disabled. Maximum MSG size: 256 MB; encrypted messages, PST/OST and OLE objects are not supported.

## Release files

- `MSG-Viewer-macOS.zip`: universal macOS application.
- `SHA256SUMS`: archive checksum.
- `update.json` and `update.sig`: digitally signed update metadata used by the app.

This public repository contains ready-to-install binaries and user documentation. Source code is maintained separately in a private repository. No GitHub access token or private update-signing key is included in the application.
