# DevSpace App Directory

# English (Русский язык см. ниже)

This repository contains JSON files describing applications and websites displayed on the [DevSpace](https://reaver.is-a.dev/devspace) platform by Reaver Entertainment.

## 📦 How to Add Your App or Website

Anyone can contribute by creating a JSON file with information about their app or website and submitting a **pull request**. Your application will be visible on the DevSpace page after approval.

### ✅ Requirements

- Each file must contain **one app or website** only.
- All fields are **required**.
- JSON must be valid and well-formatted.
- File must be added to the `/apps` folder.
- Add your JSON filename to the `index.json` list (also in `/apps`).

---

## 📁 JSON Templates

### Template for Apps (`"type": "app"`)

```json
{
  "name": "Your App Name",
  "type": "app",
  "description": "Short description of the app",
  "author": {
    "name": "Your name or team",
    "link": "https://github.com/your-profile"
  },
  "version": "1.0.0",
  "tags": ["tag1", "tag2", "another"],
  "platforms": ["Windows", "Linux", "Mac"],
  "screenshots": [
    "https://example.com/screenshot1.png",
    "https://example.com/screenshot2.png"
  ],
  "icon": "https://example.com/icon.png",
  "download": {
    "label": "Download .exe",
    "url": "https://example.com/app.exe"
  },
  "repo": "https://github.com/your-profile/your-repo",
  "license": "MIT",
  "lastUpdate": "2025-07-04"
}
```

---

### Template for Websites (`"type": "website"`)

```json
{
  "name": "Your Website Name",
  "type": "website",
  "description": "Site description or slogan",
  "author": {
    "name": "Your name or team",
    "link": "https://github.com/your-profile"
  },
  "version": "1.0.0",
  "tags": ["web", "chat", "pwa"],
  "platforms": ["Web", "PWA"],
  "screenshots": [
    "https://example.com/screenshot1.png"
  ],
  "icon": "https://example.com/icon.png",
  "download": {
    "label": "Open Website",
    "url": "https://example.com"
  },
  "repo": "https://github.com/your-profile/your-repo",
  "license": "GPL-3.0",
  "lastUpdate": "2025-07-04"
}
```

---

## 📄 Example of `index.json`

```json
[
  "reavervpn.json",
  "element-messenger.json"
]
```

> `index.json` must be in the same folder as your app files (`/apps/`), and it should include the filename of every JSON app you want listed on the site.

---

## 📘 Field Reference

| Field             | Type     | Description                                |
|------------------|----------|--------------------------------------------|
| `name`           | string   | App or website name                        |
| `type`           | string   | `"app"` or `"website"`                     |
| `description`    | string   | Short summary                              |
| `author.name`    | string   | Author or team name                        |
| `author.link`    | string   | Link to GitHub or personal site            |
| `version`        | string   | Current version                            |
| `tags`           | array    | Keywords and topics                        |
| `platforms`      | array    | Supported platforms (e.g. Windows, Web)    |
| `screenshots`    | array    | Direct links to screenshots                |
| `icon`           | string   | Link to icon image                         |
| `download.label` | string   | Text for the download button               |
| `download.url`   | string   | URL for download or site visit             |
| `repo`           | string   | GitHub repository link                     |
| `license`        | string   | License type (MIT, GPL, etc.)              |
| `lastUpdate`     | string   | Last update date in format YYYY-MM-DD      |

---

## 🙋 Need Help?

If you're unsure how to create or submit your app JSON file, feel free to open an [issue](https://github.com/playreaver/elementapps/issues) or contact us on [Reaver.is-a.dev](https://reaver.is-a.dev/).

# Русский

# 📦 DevSpace — Платформа приложений от Reaver.Entertainment

**DevSpace** — это открытая площадка для размещения приложений, сайтов и утилит. Любой разработчик может опубликовать свой проект, добавив `.json`-файл по шаблону.

---

## 📁 Структура репозитория

Все `.json`-файлы находятся в директории [`/apps/`](./apps/).

Файл `index.json` содержит список всех подключённых JSON-файлов, которые будут отображаться на сайте:

```json
[
  "reavervpn.json",
  "element-messenger.json"
]
```

> ⚠️ **Важно:** ваш файл должен быть добавлен в `index.json`.

---

## 📄 Шаблоны JSON-файлов

### 🔹 Приложение (`type: "app"`)

```json
{
  "name": "Ваше имя приложения",
  "type": "app",
  "description": "Краткое описание приложения",
  "author": {
    "name": "Ваш ник или команда",
    "link": "https://github.com/ваш-профиль"
  },
  "version": "1.0.0",
  "tags": ["ключевое", "слово", "еще"],
  "platforms": ["Windows", "Linux", "Mac"],
  "screenshots": [
    "https://example.com/screenshot1.png"
  ],
  "icon": "https://example.com/icon.png",
  "download": {
    "label": "Скачать .exe",
    "url": "https://example.com/app.exe"
  },
  "repo": "https://github.com/ваш-профиль/репозиторий",
  "license": "MIT",
  "lastUpdate": "2025-07-04"
}
```

---

### 🔹 Веб-сайт (`type: "website"`)

```json
{
  "name": "Имя вашего сайта",
  "type": "website",
  "description": "Описание или слоган",
  "author": {
    "name": "Имя автора/команды",
    "link": "https://github.com/ваш-профиль"
  },
  "version": "1.0.0",
  "tags": ["веб", "pwa", "мессенджер"],
  "platforms": ["Web", "PWA"],
  "screenshots": [
    "https://example.com/screenshot1.png"
  ],
  "icon": "https://example.com/icon.png",
  "download": {
    "label": "Открыть сайт",
    "url": "https://example.com"
  },
  "repo": "https://github.com/ваш-профиль/репозиторий",
  "license": "GPL-3.0",
  "lastUpdate": "2025-07-04"
}
```

---

## 🧾 Поля JSON-файлов

| Поле             | Тип     | Описание                                |
|------------------|----------|------------------------------------------|
| `name`           | string   | Название приложения/сайта               |
| `type`           | string   | `"app"` или `"website"`                 |
| `description`    | string   | Краткое описание                        |
| `author.name`    | string   | Имя автора/команды                      |
| `author.link`    | string   | Ссылка на GitHub или сайт               |
| `version`        | string   | Версия приложения                       |
| `tags`           | array    | Ключевые слова                          |
| `platforms`      | array    | Поддерживаемые платформы                |
| `screenshots`    | array    | Ссылки на скриншоты                     |
| `icon`           | string   | Ссылка на иконку                        |
| `download.label` | string   | Название кнопки загрузки                |
| `download.url`   | string   | Ссылка на установщик / сайт             |
| `repo`           | string   | GitHub-репозиторий                      |
| `license`        | string   | MIT, GPL и т.д.                         |
| `lastUpdate`     | string   | Дата последнего обновления (ГГГГ-ММ-ДД) |

---

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
