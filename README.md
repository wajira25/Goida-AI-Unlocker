<div align="center">
  <span style="display: inline-block; width: 33.3%; text-align: left;">
    <a href="https://www.youtube.com/@avencores/" target="_blank">
      <img src="https://github.com/user-attachments/assets/338bcd74-e3c3-4700-87ab-7985058bd17e" alt="YouTube" height="40">
    </a>
  </span>
  <span style="display: inline-block; width: 33.3%; text-align: center;">
    <a href="https://t.me/avencoresyt" target="_blank">
      <img src="https://github.com/user-attachments/assets/939f8beb-a49a-48cf-89b9-d610ee5c4b26" alt="Telegram" height="40">
    </a>
  </span>
  <span style="display: inline-block; width: 33.3%; text-align: right;">
    <a href="https://vk.com/avencoresvk" target="_blank">
      <img src="https://github.com/user-attachments/assets/dc109dda-9045-4a06-95a5-3399f0e21dc4" alt="VK" height="40">
    </a>
  </span>
  <span style="display: inline-block; width: 33.3%; text-align: right;">
    <a href="https://dzen.ru/avencores" target="_blank">
      <img src="https://github.com/user-attachments/assets/bd55f5cf-963c-4eb8-9029-7b80c8c11411" alt="Dzen" height="40">
    </a>
  </span>
</div>

<h1 align="center">Goida AI Unlocker</h1>
<p align="center">
  Мини-утилита для Windows, позволяющая <b>в один клик разблокировать популярные сервисы</b> путём обновления файла <code>hosts</code>. Под капотом — современный PySide-интерфейс с поддержкой светлой и тёмной темы.
</p>

<p align="center">
  <a href="https://github.com/AvenCores/Goida-AI-Unlocker/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/AvenCores/Goida-AI-Unlocker?style=flat-square" alt="License"/>
  </a>
  <a href="https://github.com/AvenCores/Goida-AI-Unlocker/releases/latest">
    <img src="https://img.shields.io/github/v/release/AvenCores/Goida-AI-Unlocker?style=flat-square" alt="Latest release"/>
  </a>
  <a href="https://github.com/AvenCores/Goida-AI-Unlocker/releases">
    <img src="https://img.shields.io/github/downloads/AvenCores/Goida-AI-Unlocker/total?style=flat-square" alt="Downloads"/>
  </a>
</p>

---

## 📸 Скриншот интерфейса
<div align="center">
  <img width="420" alt="UI screenshot" src="https://github.com/user-attachments/assets/3c199b46-d1c6-4f9b-a7a0-1a7dde945817" />
</div>

---

## 🌟 Основные возможности

* 🔓 Разблокировка более 60 AI-сервисов, соцсетей, игровых и музыкальных платформ (полный список ниже).
* 🗂️ Автоматическое создание резервной копии и восстановление исходного <code>hosts</code>.
* 🎨 Поддержка тёмной/светлой темы — определяется по настройкам Windows или переключается вручную.
* 🖱️ Удобный и лаконичный интерфейс: "Установить", "Удалить", "Сменить тему" и т. д.
* ⚡️ Работа без сторонних VPN/прокси: достаточно обновить <code>hosts</code>.
* 🔒 Запрос прав администратора выполняется только на момент записи, в остальное время программа работает в обычном режиме.

---

## 🚀 Быстрый старт

### 1. Скачайте готовый релиз (рекомендуется)

1. Перейдите во вкладку <a href="https://github.com/AvenCores/Goida-AI-Unlocker/releases/latest">Releases</a>.
2. Скачайте файл с пометкой <code>.exe</code> (x64).
3. Запустите <code>Goida AI Unlocker.exe</code> от имени администратора и нажмите «Установить обход блокировок».

### 2. Запуск из исходников

```bash
# Склонируйте репозиторий
git clone https://github.com/AvenCores/Goida-AI-Unlocker.git
cd Goida-AI-Unlocker

# Установите зависимости
python -m pip install -r requirements.txt

# Запустите приложение
python main.py
```

Требования:
* Windows 10/11
* Python 3.8+

---

## 🛠️ Сборка собственного EXE

Для создания портативного одного файла используется [PyInstaller](https://pyinstaller.org/):

```bash
pyinstaller main.py --onefile --noconsole --icon=icon.ico --clean --strip --name "Goida AI Unlocker" --add-data "icon.ico;."
```

Скомпилированный файл появится в директории <code>dist/</code>.

---

## 🧩 Как это работает
Приложение скачивает свежий файл <code>hosts</code> из репозитория <a href="https://github.com/ImMALWARE/dns.malw.link">dns.malw.link</a> и заменяет системный <code>C:\Windows\System32\drivers\etc\hosts</code>. При необходимости предыдущая версия автоматически сохраняется и может быть восстановлена кнопкой «Удалить обход блокировок».

> ⚠️ Изменение <code>hosts</code> может повлиять на работу некоторых корпоративных VPN/прокси. Если возникнут проблемы — воспользуйтесь кнопкой «Удалить обход блокировок» или вручную верните оригинальный файл.

---

## 🌍 Разблокируемые сервисы

### 📱 Социальные сети и мессенджеры
* Instagram · TikTok · Truth Social · Guilded

### 🧠 AI-платформы
* ChatGPT / OpenAI (включая Sora) · Claude · Grok · Gemini · Google AI Studio · NotebookLM · Google Labs (Jules, Stitch и др.) · Microsoft Copilot · GitHub Copilot · ElevenLabs · DeepL

### 🎮 Игры и игровые сервисы
* Clash Royale · Clash of Clans · Brawl Stars · Supercell (ассеты) · Xbox · Xbox Cloud Gaming · Microsoft Rewards

### 🎵 Музыкальные сервисы
* Spotify · Tidal · Deezer

### ✉️ Электронная почта и облако
* Proton Mail · Proton Drive

### 🧩 Разработка и программирование
* GitHub (включая Copilot API) · JetBrains (Datalore, Plugins) · Google AI API · NVIDIA Developer · Parsec

### 🛠️ Продуктивность и утилиты
* Notion · Canva · Intel · Dell · Weather.com · Imgur · Web Archive · Tria.ge

### ⌚️ Здоровье и фитнес
* Fitbit

### 💳 Финансы
* Square / Squareup (через Tidal)

### 🌐 Торренты
* OpenBitTorrent (tracker.openbittorrent.com)

### 🚫 Блокировка вредных сайтов
* Скримеры: <code>only-fans.uk</code>, <code>only-fans.me</code>, <code>onlyfans.wtf</code>
* IP-логгеры: <code>iplogger.org</code>, <code>wl.gl</code>, <code>ed.tc</code>, <code>bc.ax</code>, <code>maper.info</code>, <code>2no.co</code>, <code>yip.su</code>, <code>iplis.ru</code>, <code>ezstat.ru</code>, <code>iplog.co</code>, <code>grabify.org</code>

---

## 💬 Вклад и обратная связь
* Нашли новую заблокированную площадку? Открывайте <a href="https://github.com/AvenCores/Goida-AI-Unlocker/issues/new">issue</a> или отправляйте PR.
* Ошибка или неожиданное поведение? Пожалуйста, оформите подробный баг-репорт.
* Буду рад вашим идеям и предложениям!

---

## 💰 Поддержать автора
* **SBER**: <code>2202 2050 7215 4401</code>

---

## 📜 Лицензия
Данный проект распространяется под лицензией MIT — подробности см. в файле [LICENSE](LICENSE).
