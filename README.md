# [DevSpace](https://devspace.reaver.is-a.dev/)

# DevSpace JSON File Schema Documentation

This guide provides a detailed explanation of how to format the JSON file required for submitting a project to DevSpace.

---

## English

### Basic Information

- `"name"`: Name of your application.
  - Type: `string`
  - Example: `"My Awesome App"`

- `"description"`: Short summary of the project (supports Markdown).
  - Type: `string`
  - Example: `"Description (Markdown supported)"`

- `"type"`: Category of the project. 
  - Example: `"app"`, `"website"`

- `"version"`: App version, preferably in Semantic Versioning.
  - Example: `"1.0.0"`

- `"license"`: The license under which the project is released.
  - Example: `"MIT"`

- `"lastUpdate"`: Last update date in format `DD/MM/YYYY`.
  - Example: `"09/07/2025"`

- `"icon"`: URL to an icon representing the app.
  - Example: `"https://example.com/icon.png"`

- `"repo"`: Link to the source code repository.
  - Example: `"https://github.com/user/repo"`

- `"docs"`: Documentation URL or `"none"` if unavailable.
  - Example: `"https://example.com/docs"`

- `"video"`: YouTube or similar demo video URL.
  - Example: `"https://youtube.com/demo"`

### Author

- `"author"`:
  - `"name"`: Author's name.
  - `"link"`: Author's website or profile URL.

### Languages

- `"languages"`: Array of supported languages (programming or spoken).
  - Example: `["JavaScript", "English"]`

### Platforms

- `"platforms"`: Supported operating systems or browsers.
  - Example: `["Windows", "Linux", "Web", "Google Chrome"]`

### Tags

- `"tags"`: Tag categories:

  - `"type"`: 
    - Values like `"Library"`, `"App"`, `"Package"`, etc.

  - `"purpose"`: 
    - For example: `"Frontend"`, `"Backend"`, `"Education"`

  - `"technology"`: 
    - Technologies used: `"JavaScript"`, `"React"`, `"Python"`

  - `"functionality"`: 
    - Features like `"Authentication"`, `"Analytics"`

  - `"maturity"`: 
    - Development stage: `"Alpha"`, `"Stable"`

  - `"other"`: 
    - Extra tags like `"Offline"`, `"Mobile Ready"`

### Download

- `"download"`:
  - `"url"`: Link to download or open the app.
  - `"label"`: Label shown on the download button.

### Contributors

- `"contributors"`: List of contributors.
  - Each has:
    - `"name"`: Contributor’s name
    - `"role"`: Role in the project
    - `"avatar"`: URL to their avatar
    - `"link"`: Profile URL

### Roadmap

- `"roadmap"`: Planned features or goals.
  - Each entry:
    - `"title"`: Name of feature
    - `"description"`: Description of the task or feature

### Changelog

- `"changelog"`: Key-value list of version changes.
  - Key: version number
  - Value: changelog description

---

## 🚀 How to Publish Your Project

1. **Fork this repository**:  
   👉 [https://github.com/playreaver/elementapps](https://github.com/playreaver/elementapps)

2. Inside the `/apps/` folder:
   - Create your own `yourapp.json` file based on the template
   - Add your filename to `index.json`

3. **Submit a Pull Request** with a description like:  
   _"Added application: MyCoolApp"_

4. We will review and publish your project on [**reaver.is-a.dev**](https://reaver.is-a.dev) under the **DevSpace** section.

---

## ✅ Recommendations

- Use **direct links** to images and files
- Make sure all links are **working**
- Validate your JSON structure using a tool like [jsonlint.com](https://jsonlint.com)

---

## 🛠 Feedback

If you have any questions, open an [Issue](https://github.com/playreaver/elementapps/issues) or leave a comment in your Pull Request.

Welcome to **DevSpace** by [Reaver.Entertainment](https://reaver.is-a.dev)!

---

## Русский

### Основная информация

- `"name"`: Название вашего приложения.
  - Тип: `string`
  - Пример: `"My Awesome App"`

- `"description"`: Краткое описание проекта (поддерживается Markdown).
  - Тип: `string`
  - Пример: `"Description (Markdown supported)"`

- `"type"`: Тип проекта.
  - Пример: `"app"`, `"website"`

- `"version"`: Версия приложения (желательно в формате SemVer).
  - Пример: `"1.0.0"`

- `"license"`: Лицензия, по которой распространяется проект.
  - Пример: `"MIT"`

- `"lastUpdate"`: Дата последнего обновления в формате `ДД/ММ/ГГГГ`.
  - Пример: `"09/07/2025"`

- `"icon"`: Ссылка на иконку проекта.
  - Пример: `"https://example.com/icon.png"`

- `"repo"`: Ссылка на репозиторий исходного кода.
  - Пример: `"https://github.com/user/repo"`

- `"docs"`: Ссылка на документацию или `"none"`, если её нет.
  - Пример: `"https://example.com/docs"`

- `"video"`: Ссылка на демонстрационное видео (например, YouTube).
  - Пример: `"https://youtube.com/demo"`

### Автор

- `"author"`:
  - `"name"`: Имя автора
  - `"link"`: Сайт или профиль автора

### Языки

- `"languages"`: Массив поддерживаемых языков (программирования или интерфейса).
  - Пример: `["JavaScript", "English"]`

### Платформы

- `"platforms"`: Поддерживаемые ОС и браузеры.
  - Пример: `["Windows", "Linux", "Web", "Google Chrome"]`

### Теги

- `"tags"`: Категории меток:

  - `"type"`: 
    - Например: `"Library"`, `"App"`, `"Package"`

  - `"purpose"`: 
    - Назначение: `"Frontend"`, `"Backend"`, `"Education"`

  - `"technology"`: 
    - Технологии: `"React"`, `"Python"`, `"Vue"`

  - `"functionality"`: 
    - Функциональность: `"Authentication"`, `"Analytics"`

  - `"maturity"`: 
    - Этап зрелости проекта: `"Alpha"`, `"Stable"`

  - `"other"`: 
    - Дополнительно: `"Offline"`, `"Experimental"`

### Загрузка

- `"download"`:
  - `"url"`: Ссылка на загрузку или сайт.
  - `"label"`: Надпись на кнопке загрузки.

### Участники

- `"contributors"`: Список участников проекта.
  - Каждый содержит:
    - `"name"`: Имя
    - `"role"`: Роль
    - `"avatar"`: Ссылка на аватар
    - `"link"`: Профиль/сайт

### План разработки

- `"roadmap"`: Будущие функции и цели.
  - Каждая запись:
    - `"title"`: Название
    - `"description"`: Описание задачи

### История изменений

- `"changelog"`: Список изменений по версиям.
  - Ключ: номер версии
  - Значение: описание изменений


## 🚀 Как опубликовать свой проект

1. **Сделайте Fork** этого репозитория:  
   👉 [https://github.com/playreaver/elementapps](https://github.com/playreaver/elementapps)

2. В папке `/apps/`:
   - Создайте свой файл `yourapp.json` по шаблону
   - Добавьте имя файла в `index.json`

3. **Сделайте Pull Request** с описанием:  
   _"Добавлено приложение: MyCoolApp"_

4. Мы проверим и опубликуем ваш проект на [**reaver.is-a.dev**](https://reaver.is-a.dev) в разделе **DevSpace**.

---

## ✅ Рекомендации

- Используйте **прямые ссылки** на изображения и файлы
- Убедитесь, что все ссылки **работают**
- Проверяйте структуру JSON на валидность, например на [jsonlint.com](https://jsonlint.com)

---

## 🛠 Обратная связь

Если у вас возникли вопросы — откройте [Issue](https://github.com/playreaver/elementapps/issues) или напишите в Pull Request.

Добро пожаловать в **DevSpace** от [Reaver.Entertainment](https://reaver.is-a.dev)!
