## Tg2VkColab

![](/example.jpg)
![](/example2.jpg)
![](/example3.jpg)

### Project Description

**Tg2VkColab** is a software project designed to automate and simplify the process of transferring media content from Telegram to the VKontakte social network. The project enables users to automatically send messages and media files from a specified Telegram channel or chat to a designated VKontakte page or group. This version is specifically adapted for use with Google Colab, making it easier to run the project in a cloud-based environment.

### Purpose of the Project

Many users and community administrators face the need to duplicate content across different platforms. This task can be routine and time-consuming. Tg2VkColab automates this process, saving time and reducing the likelihood of errors that can occur when copying data manually.

### How Tg2VkColab Works

1. **Data Retrieval from Telegram**: The project uses the `aiogram` library to interact with the Telegram API. This allows for the retrieval of messages and media files from specified chats or channels.
2. **Media Content Processing**: With the help of `aiogram-media-group`, `moviepy`, and `rlottie-python`, media files are processed and prepared for further transmission.
3. **Data Sending to VKontakte**: The `vk-api` library is used to interact with the VKontakte API, enabling the upload and sending of media files and messages to specified pages or groups.

### Supported Media Files

Tg2VkColab is designed to transfer various types of media files from Telegram to VKontakte, including:

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
   - Groups of media files, including combinations of images and videos, sent as a single message.

### Example Usage

- **Images**: If a user sends a photo with a description in Telegram, the bot automatically forwards the image and text to the specified VKontakte page or group.
- **Videos**: Videos from Telegram are forwarded in the appropriate format to VKontakte, preserving the original quality.
- **Documents**: Important files or documents are forwarded for convenient access by VKontakte group members.
- **Voice Messages**: Voice recordings from Telegram are forwarded as audio files to VKontakte.

### Installation and Launch

To set up and run the Tg2VkColab project in Google Colab, follow these steps:

1. **Clone the Repository**:

   ```bash
   !git clone https://github.com/ring-rong/Tg2VkColab.git
   %cd Tg2VkColab
   ```

2. **Install Necessary Dependencies**:

   Ensure that `pip` is installed. Then run the following command:

   ```bash
   !pip install -r requirements.txt
   ```

3. **Environment Setup**:

   ```
   VK_API_TOKEN=YOUR_VK_API_TOKEN
   TELEGRAM_API_TOKEN=YOUR_TELEGRAM_API_TOKEN
   TELEGRAM_CHANNEL_USERNAME=YOUR_TELEGRAM_CHANNEL_USERNAME
   VK_GROUP_ID=YOUR_VK_GROUP_ID
   ```

4. **Run the Application**:

   The application can be launched with the following command:

   ```bash
   !python app.py
   ```

### Detailed Implementation

- **`aiogram`**: An asynchronous library for working with the Telegram Bot API.
- **`aiogram-media-group`**: An extension for handling group media messages in Telegram.
- **`aiohttp`**: An asynchronous HTTP client/server library.
- **`python-dotenv`**: Allows loading environment variables from a `.env` file.
- **`vk-api`**: A library for interacting with the VKontakte API.
- **`rlottie-python`**: A library for working with animations.
- **`moviepy`**: A library for video editing.
- **`requests`**: A simple HTTP library for Python.
- **`nest_asyncio`**: Allows the use of asyncio in environments that don't support it natively.

By supporting a wide range of media files, Tg2VkColab ensures flexibility and convenience when transferring content between platforms. This Google Colab version allows users to leverage cloud-based resources for easier setup and execution.

--------------------------------------------------------------------------------------------

## Tg2VkColab

![](/example.jpg)
![](/example2.jpg)
![](/example3.jpg)

### Описание проекта

**Tg2VkColab** — это программный проект, созданный для автоматизации и упрощения процесса переноса медиа-контента из Telegram в социальную сеть ВКонтакте. Проект позволяет пользователям автоматически отправлять сообщения и медиафайлы из определенного Telegram-канала или чата на заданную страницу или группу ВКонтакте. Эта версия специально адаптирована для использования с Google Colab, что облегчает запуск проекта в облачной среде.

### Зачем нужен этот проект

Многие пользователи и администраторы сообществ сталкиваются с необходимостью дублирования контента между различными платформами. Это может быть рутинной и трудоемкой задачей. Tg2VkColab автоматизирует этот процесс, экономя время и уменьшая вероятность ошибок при копировании данных вручную.

### Как работает Tg2VkColab

1. **Получение данных из Telegram**: Проект использует библиотеку `aiogram` для взаимодействия с Telegram API. Это позволяет получать сообщения и медиафайлы из указанных чатов или каналов.
2. **Обработка медиа-контента**: С помощью `aiogram-media-group`, `moviepy` и `rlottie-python` происходит обработка и подготовка медиафайлов для дальнейшей отправки.
3. **Отправка данных в ВКонтакте**: Библиотека `vk-api` используется для взаимодействия с API ВКонтакте, что позволяет загружать и отправлять медиафайлы и сообщения на указанные страницы или группы.

### Поддерживаемые медиафайлы

Tg2VkColab предназначен для пересылки различных типов медиафайлов из Telegram в ВКонтакте, включая:

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
- **Видео**: Видео из Telegram пересылается в соответствующем формате в ВКонтакте, сохраняя оригинальное качество.
- **Документы**: Важные файлы или документы пересылаются для удобного доступа участников группы ВКонтакте.
- **Голосовые сообщения**: Голосовые записи из Telegram пересылаются как аудиофайлы в ВКонтакте.

### Установка и запуск

Чтобы настроить и запустить проект Tg2VkColab в Google Colab, выполните следующие шаги:

1. **Склонируйте репозиторий**:

   ```bash
   !git clone https://github.com/ring-rong/Tg2VkColab.git
   %cd Tg2VkColab
   ```

2. **Установите необходимые зависимости**:

   Убедитесь, что у вас установлен `pip`. Затем выполните команду:

   ```bash
   !pip install -r requirements.txt
   ```

3. **Настройка окружения**:

   ```env
   VK_API_TOKEN=YOUR_VK_API_TOKEN
   TELEGRAM_API_TOKEN=YOUR_TELEGRAM_API_TOKEN
   TELEGRAM_CHANNEL_USERNAME=YOUR_TELEGRAM_CHANNEL_USERNAME
   VK_GROUP_ID=YOUR_VK_GROUP_ID
   ```

4. **Запуск приложения**:

   Приложение можно запустить с помощью следующей команды:

   ```bash
   !python app.py
   ```

### Подробности реализации

- **`aiogram`**: Асинхронная библиотека для работы с Telegram Bot API.
- **`aiogram-media-group`**: Расширение для обработки групповых медиа-сообщений в Telegram.
- **`aiohttp`**: Асинхронная библиотека HTTP-клиента/сервера.
- **`python-dotenv`**: Позволяет загружать переменные окружения из файла `.env`.
- **`vk-api`**: Библиотека для работы с API ВКонтакте.
- **`rlottie-python`**: Библиотека для работы с анимациями.
- **`moviepy`**: Библиотека для редактирования видео.
- **`requests`**: Простая HTTP-библиотека для Python.
- **`nest_asyncio`**: Позволяет использовать asyncio в средах, которые не поддерживают его нативно.

Поддерживая широкий спектр медиафайлов, Tg2VkColab обеспечивает гибкость и удобство при переносе контента между платформами. Эта версия для Google Colab позволяет пользователям использовать облачные ресурсы для более легкой настройки и выполнения.
