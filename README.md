### Проект Tg2Vk

![](/example.jpg)
![](/example2.jpg)
![](/example3.jpg)

#### Описание проекта

**Tg2Vk** — это программный проект, созданный для автоматизации и упрощения процесса переноса медиа-контента из Telegram в социальную сеть ВКонтакте. Проект позволяет пользователям автоматически отправлять сообщения и медиафайлы из определенного Telegram-канала или чата на заданную страницу или группу ВКонтакте.

#### Зачем нужен этот проект

Многие пользователи и администраторы сообществ сталкиваются с необходимостью дублирования контента между различными платформами. Это может быть рутинной и трудоемкой задачей. Tg2Vk автоматизирует этот процесс, экономя время и уменьшая вероятность ошибок при копировании данных вручную. 

#### Как работает Tg2Vk

1. **Получение данных из Telegram:** Проект использует библиотеку `aiogram` для взаимодействия с Telegram API. Это позволяет получать сообщения и медиафайлы из указанных чатов или каналов.
2. **Обработка медиа-контента:** С помощью `aiogram-media-group`, `moviepy` и `rlottie-python` происходит обработка и подготовка медиафайлов для дальнейшей отправки.
3. **Отправка данных в ВКонтакте:** Библиотека `vk-api` используется для взаимодействия с API ВКонтакте, что позволяет загружать и отправлять медиафайлы и сообщения на указанные страницы или группы.
4. **Конфигурация и управление:** Файл `.env` используется для хранения конфиденциальных данных и ключей API, обеспечивая безопасное управление параметрами приложения.

### Какие медиафайлы может пересылать бот Tg2Vk

Бот Tg2Vk предназначен для пересылки различных типов медиафайлов из Telegram в ВКонтакте. Вот список медиафайлов, которые бот может обрабатывать и пересылать:

1. **Текстовые сообщения**:
   - Простые текстовые сообщения без медиафайлов.

2. **Изображения**:
   - Фотографии в различных форматах (JPEG, PNG и др.).

3. **Видео**:
   - Видеофайлы в популярных форматах (MP4 и др.).

4. **Аудио**:
   - Голосовые сообщения и музыкальные файлы.

5. **Документы**:
   - Файлы различных типов, включая PDF, DOCX, XLSX и другие.

6. **Анимации**:
   - GIF-анимации и анимированные стикеры.

7. **Медиа-группы**:
   - Группы медиафайлов, включающие комбинации изображений и видео, отправленные как единое сообщение.

### Пример использования

- **Изображения**: Если пользователь отправляет в Telegram фото с описанием, бот автоматически пересылает это изображение и текст на указанную страницу или группу ВКонтакте.
- **Видео**: Видео с Telegram пересылается в соответствующем формате в ВКонтакте, сохраняя оригинальное качество.
- **Документы**: Важные файлы или документы пересылаются для удобного доступа участников группы ВКонтакте.
- **Голосовые сообщения**: Голосовые записи из Telegram пересылаются как аудиофайлы в ВКонтакте.

Таким образом, Tg2Vk поддерживает широкий спектр медиафайлов, обеспечивая гибкость и удобство при переносе контента между платформами.

#### Установка и запуск проекта

1. **Склонируйте репозиторий:**

   ```bash
   git clone https://github.com/ring-rong/Tg2Vk.git
   cd Tg2Vk
   ```

2. **Установите необходимые зависимости:**

   Убедитесь, что у вас установлен `pip`. Затем выполните команду:

   ```bash
   pip install -r requirements.txt
   ```

3. **Настройка окружения:**

   Создайте файл `.env` в корне проекта и добавьте необходимые переменные окружения. Пример файла `.env`:

   ```env
   VK_API_TOKEN=YOUR_VK_API_TOKEN
   TELEGRAM_API_TOKEN=YOUR_TELEGRAM_API_TOKEN
   TELEGRAM_CHANNEL_USERNAME=YOUR_TELEGRAM_CHANNEL_USERNAME
   VK_GROUP_ID=YOUR_VK_GROUP_ID
   ```

4. **Запуск приложения:**

   Приложение можно запустить с помощью следующей команды:

   ```bash
   python app.py
   ```

#### Подробности реализации

- **`aiogram`**: Асинхронная библиотека для работы с Telegram Bot API.
- **`aiogram-media-group`**: Расширение для обработки групповых медиа-сообщений в Telegram.
- **`aiohttp`**: Асинхронная библиотека HTTP-клиента/сервера.
- **`python-dotenv`**: Позволяет загружать переменные окружения из файла `.env`.
- **`vk-api`**: Библиотека для работы с API ВКонтакте.
- **`rlottie-python`**: Библиотека для работы с анимациями.
- **`moviepy`**: Библиотека для редактирования видео.



-------------------------------------------------------------------------------------------------------------------------------------------------------------------------


### Project Tg2Vk

![](/example.jpg)
![](/example2.jpg)
![](/example3.jpg)

#### Project Description

**Tg2Vk** is a software project designed to automate and simplify the process of transferring media content from Telegram to the social network VKontakte. The project allows users to automatically send messages and media files from a specified Telegram channel or chat to a designated VKontakte page or group.

#### Why This Project is Needed

Many users and community administrators face the need to duplicate content across different platforms. This can be a routine and time-consuming task. Tg2Vk automates this process, saving time and reducing the likelihood of errors when copying data manually.

#### How Tg2Vk Works

1. **Data Retrieval from Telegram:** The project uses the `aiogram` library to interact with the Telegram API, allowing it to fetch messages and media files from specified chats or channels.
2. **Media Content Processing:** Using `aiogram-media-group`, `moviepy`, and `rlottie-python`, media files are processed and prepared for further uploading.
3. **Data Sending to VKontakte:** The `vk-api` library is used to interact with the VKontakte API, enabling the upload and posting of media files and messages to specified pages or groups.
4. **Configuration and Management:** A `.env` file is used to store sensitive data and API keys, ensuring secure management of application parameters.

### Types of Media Files Tg2Vk Bot Can Transfer

The Tg2Vk bot is designed to transfer various types of media files from Telegram to VKontakte. Here is a list of media files that the bot can handle and transfer:

1. **Text Messages**:
   - Simple text messages without media files.

2. **Images**:
   - Photos in various formats (JPEG, PNG, etc.).

3. **Videos**:
   - Video files in popular formats (MP4, etc.).

4. **Audio**:
   - Voice messages and music files.

5. **Documents**:
   - Files of various types, including PDF, DOCX, XLSX, and others.

6. **Animations**:
   - GIF animations and animated stickers.

7. **Media Groups**:
   - Groups of media files, including combinations of images and videos sent as a single message.

### Example of Use

- **Images**: If a user sends a photo with a caption in Telegram, the bot automatically transfers this image and text to the specified VKontakte page or group.
- **Videos**: Videos from Telegram are transferred in the corresponding format to VKontakte, preserving the original quality.
- **Documents**: Important files or documents are transferred for easy access by VKontakte group members.
- **Voice Messages**: Voice recordings from Telegram are transferred as audio files to VKontakte.

Thus, Tg2Vk supports a wide range of media files, providing flexibility and convenience when transferring content between platforms.

#### Installation and Running the Project

1. **Clone the repository:**

   ```bash
   git clone https://github.com/ring-rong/Tg2Vk.git
   cd Tg2Vk
   ```

2. **Install the necessary dependencies:**

   Make sure you have `pip` installed. Then run:

   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the environment:**

   Create a `.env` file in the project's root directory and add the necessary environment variables. Example of a `.env` file:

   ```env
   VK_API_TOKEN=YOUR_VK_API_TOKEN
   TELEGRAM_API_TOKEN=YOUR_TELEGRAM_API_TOKEN
   TELEGRAM_CHANNEL_USERNAME=YOUR_TELEGRAM_CHANNEL_USERNAME
   VK_GROUP_ID=YOUR_VK_GROUP_ID
   ```

4. **Run the application:**

   You can run the application with the following command:

   ```bash
   python app.py
   ```

#### Implementation Details

- **`aiogram`**: Asynchronous library for working with the Telegram Bot API.
- **`aiogram-media-group`**: Extension for handling media group messages in Telegram.
- **`aiohttp`**: Asynchronous HTTP client/server library.
- **`python-dotenv`**: Allows loading environment variables from a `.env` file.
- **`vk-api`**: Library for working with the VKontakte API.
- **`rlottie-python`**: Library for working with animations.
- **`moviepy`**: Library for video editing.
