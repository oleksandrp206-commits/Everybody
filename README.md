# Портфолио «Орлов — Frontend, выпуск №05»

Одностраничный сайт-портфолио в виде асимметричного журнального макета с неоновым градиентом. Один файл: `portfolio-v2.html` — HTML, CSS и JavaScript собраны вместе, никаких сборщиков и зависимостей не нужно.

## Быстрый старт

1. Скачайте файл `portfolio-v2.html`.
2. Откройте его двойным кликом в любом браузере (Chrome, Firefox, Safari, Edge) — сайт заработает сразу, без сервера.
3. Чтобы разместить сайт в интернете, загрузите этот же файл на любой статический хостинг: GitHub Pages, Netlify, Vercel, Cloudflare Pages и т.п. Файл нужно переименовать в `index.html`.

## Что внутри

- **Переключатель языка (RU / EN)** — кнопка в шапке, текст сайта хранится в JS-объекте `dict` и переключается без перезагрузки страницы.
- **Переключатель темы (тёмная / светлая)** — управляется атрибутом `data-theme` на `<html>`.
- Выбранные язык и тема сохраняются в `localStorage` браузера — при повторном визите настройки не сбрасываются.
- Секции: заголовок-шапка, обложка (hero) с заголовком и статусом, оглавление, «Работы» (проекты), «Инструменты», «Заметки», «Контакты», подвал.

## Как отредактировать содержимое

Весь текст сайта на двух языках лежит в одном месте — объекте `dict` в конце файла (внутри тега `<script>`). Чтобы поменять текст:

1. Откройте `portfolio-v2.html` в любом текстовом редакторе (VS Code, Sublime, обычный «Блокнот»).
2. Найдите строку `var dict = {`.
3. Каждая запись выглядит так: `ключ: { ru:"русский текст", en:"english text" }`. Меняйте текст внутри кавычек — структуру трогать не нужно.
4. Названия проектов (Nimbus, Fielddesk), стек технологий, ссылки (email, GitHub, Telegram) написаны прямо в HTML-разметке — их можно найти по названию через поиск (Ctrl+F) и заменить.

## Как поменять цвета

В начале файла, в блоке `<style>`, есть секция `:root { ... }` — там заданы все цвета сайта через CSS-переменные (`--bg`, `--pink`, `--violet`, `--cyan` и другие). Для светлой темы такой же набор переменных задан отдельно в `:root[data-theme="light"] { ... }`. Меняя эти значения, вы меняете палитру сразу по всему сайту.

## Технологии

Чистый HTML5, CSS3 (Grid, CSS-переменные, градиенты) и vanilla JavaScript. Шрифты Fraunces и Manrope подключены через Google Fonts. Фреймворки и сборка не требуются.

---

# "Orlov — Frontend, Issue №05" Portfolio

A single-page portfolio site styled as an asymmetric magazine layout with a neon gradient. One file: `portfolio-v2.html` — HTML, CSS and JavaScript are all bundled together, no build tools or dependencies required.

## Quick start

1. Download the `portfolio-v2.html` file.
2. Double-click to open it in any browser (Chrome, Firefox, Safari, Edge) — the site works immediately, no server needed.
3. To publish it online, upload the same file to any static hosting service: GitHub Pages, Netlify, Vercel, Cloudflare Pages, etc. Rename the file to `index.html`.

## What's inside

- **Language switch (RU / EN)** — a button in the header; site text lives in a JS object called `dict` and switches instantly without reloading the page.
- **Theme switch (dark / light)** — controlled via the `data-theme` attribute on `<html>`.
- The chosen language and theme are saved in the browser's `localStorage`, so they persist on return visits.
- Sections: header, hero (headline + status), table of contents, "Work" (projects), "Toolkit", "Notes", "Contact", footer.

## How to edit the content

All site text in both languages lives in one place — the `dict` object near the end of the file (inside the `<script>` tag). To change the text:

1. Open `portfolio-v2.html` in any text editor (VS Code, Sublime, even plain Notepad).
2. Find the line `var dict = {`.
3. Each entry looks like: `key: { ru:"russian text", en:"english text" }`. Edit the text inside the quotes — no need to touch the structure.
4. Project names (Nimbus, Fielddesk), the tech stack, and links (email, GitHub, Telegram) are written directly in the HTML markup — find them with search (Ctrl+F) and replace as needed.

## How to change the colors

Near the top of the file, inside the `<style>` block, there's a `:root { ... }` section defining all site colors as CSS variables (`--bg`, `--pink`, `--violet`, `--cyan`, and others). The light theme has its own matching set defined separately in `:root[data-theme="light"] { ... }`. Editing these values updates the palette across the entire site.

## Tech stack

Plain HTML5, CSS3 (Grid, CSS variables, gradients) and vanilla JavaScript. Fraunces and Manrope fonts are loaded via Google Fonts. No frameworks or build step required.
