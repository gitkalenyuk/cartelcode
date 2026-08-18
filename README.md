<div align="center">

<img src="https://raw.githubusercontent.com/gitkalenyuk/cartelcode/main/.github/logo.svg" width="88" alt="Cartel Code" />

# Cartel Code

### Пише, читає й править код разом з вами

Портативний агент для коду з власним шлюзом API, пулом ключів, 168 плагінами<br>і повністю українською оболонкою. Node і Electron уже всередині.

<br>

[![Завантажити для Windows](https://img.shields.io/badge/Завантажити-Windows%20x64-ff7a3d?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/gitkalenyuk/cartelcode/releases/latest)
[![Завантажити для macOS](https://img.shields.io/badge/Завантажити-macOS-ff7a3d?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/gitkalenyuk/cartelcode/releases/latest)

[![Версія](https://img.shields.io/github/v/release/gitkalenyuk/cartelcode?style=flat-square&color=ff7a3d&label=версія)](https://github.com/gitkalenyuk/cartelcode/releases/latest)
[![Завантажень](https://img.shields.io/github/downloads/gitkalenyuk/cartelcode/total?style=flat-square&color=ff7a3d&label=завантажень)](https://github.com/gitkalenyuk/cartelcode/releases)
[![Канал](https://img.shields.io/badge/Telegram-канал-2aabee?style=flat-square&logo=telegram&logoColor=white)](https://t.me/YT_cartell)
[![Чат](https://img.shields.io/badge/Telegram-чат-2aabee?style=flat-square&logo=telegram&logoColor=white)](https://t.me/+Ovf7rTg8ClBkOGQy)

**[Сайт проєкту →](https://gitkalenyuk.github.io/cartelcode/)**  ·  **[Довідка →](https://gitkalenyuk.github.io/cartelcode/docs.html)**

</div>

---

## Завантажити

| Система | Файл | Розмір |
|:--|:--|:--|
| **Windows 10/11** (x64) | **[CartelCode-Setup-1.0.3.exe](https://github.com/gitkalenyuk/cartelcode/releases/download/v1.0.3/CartelCode-Setup-1.0.3.exe)** | 146 МБ |
| **macOS** (Apple Silicon) | **[CartelCode-1.0.3-arm64.dmg](https://github.com/gitkalenyuk/cartelcode/releases/download/v1.0.3/CartelCode-1.0.3-arm64.dmg)** | 174 МБ |
| **macOS** (Intel) | **[CartelCode-1.0.3-x64.dmg](https://github.com/gitkalenyuk/cartelcode/releases/download/v1.0.3/CartelCode-1.0.3-x64.dmg)** | 176 МБ |

Усі файли й контрольні суми — на [сторінці релізів](https://github.com/gitkalenyuk/cartelcode/releases).

---

## Доступ

Вхід у застосунок — **тільки через Telegram**. Ані пароля, ані пошти. Щоб застосунок запустився, треба бути учасником **обох** спільнот:

- **[YT Cartel — канал](https://t.me/YT_cartell)**
- **[YT Cartel — чат](https://t.me/+Ovf7rTg8ClBkOGQy)**

При першому запуску відкриється сторінка входу Telegram. Пароль ми не бачимо — лише підтвердження від самого Telegram.

---

## Що всередині

### Шлюз API з пулом ключів
Кілька ключів на одного провайдера, ротація по колу між живими. Вичерпав квоту — ключ заморожується, запит іде на наступний. Заморожений ключ згодом отримує перевірочний запит і автоматично повертається до роботи. Нічого не перемикати вручну посеред задачі.

### 168 плагінів
Веб-пошук для агента, бічна панель з файловим провідником і вбудованим терміналом, відмотування діалогу разом з файлами, імпорт сесій, редагування надісланих повідомлень. Кожен плагін вмикається одним перемикачем і має опис прямо в інтерфейсі.

### Український інтерфейс
Не машинний переклад поверх англійського: меню, підказки, стани, повідомлення про помилки й описи плагінів. English лишається перемикачем.

### Повна портативність
Node і Electron лежать усередині збірки. Системні версії не чіпаються, PATH не змінюється, у реєстр нічого не пишеться. Профілі, історія, ключі й плагіни живуть у теці даних застосунку.

### Оновлення без клопоту
Застосунок сам перевіряє релізи на GitHub. Файл завантажується лише з `github.com`, а перед запуском звіряються розмір і SHA-256 — якщо контрольної суми немає або вона не збіглася, оновлення скасовується.

---

## Три кроки до старту

**1. Завантажте збірку** — для Windows файл `.exe` за посиланням вище.

**2. Встановіть і відкрийте** — оберіть теку без кирилиці й пробілів у шляху.

**3. Увійдіть і оберіть проєкт** — підтвердьте акаунт Telegram, вкажіть робочу теку, і можна писати перший запит.

Встановлювати нічого не треба: ні Node.js, ні Python, ні Git.

---

## Питання

<details>
<summary><b>Чи потрібен встановлений Node.js або щось іще?</b></summary><br>
Ні. Портативні Node.js і Electron лежать усередині збірки. Системні версії не чіпаються, PATH не змінюється.
</details>

<details>
<summary><b>Де зберігаються мої дані та ключі?</b></summary><br>
Локально, у теці даних застосунку: профілі, історія сесій, API-ключі, плагіни. Запити йдуть напряму до провайдера через локальний шлюз на <code>1.0.3.1</code> — ми їх не бачимо й не проксуємо.
</details>

<details>
<summary><b>Windows каже, що видавця не перевірено</b></summary><br>
Збірка не підписана сертифікатом коду. У вікні SmartScreen: «Докладніше» → «Виконати попри все». Контрольну суму можна звірити самостійно:<br><br>
<code>Get-FileHash CartelCode-Setup-1.0.3.exe -Algorithm SHA256</code><br><br>
Очікуване значення опубліковане в <a href="https://github.com/gitkalenyuk/cartelcode/releases/latest">релізі</a> у файлі <code>.sha256</code>.
</details>

<details>
<summary><b>macOS каже, що застосунок від невідомого розробника</b></summary><br>
Права кнопка → «Відкрити». Якщо блокує: «Системні параметри» → «Конфіденційність і безпека» → «Усе одно відкрити».
</details>

<details>
<summary><b>Що потрібно для доступу?</b></summary><br>
Членство в обох спільнотах YT Cartel — <a href="https://t.me/YT_cartell">каналі</a> та <a href="https://t.me/+Ovf7rTg8ClBkOGQy">чаті</a>. Після підтвердження доступ лишається на пристрої; якщо вийти зі спільноти, застосунок попросить увійти знову.
</details>

<details>
<summary><b>Як оновлюється застосунок?</b></summary><br>
У меню внизу бічної панелі — «Перевірити оновлення». Застосунок читає релізи GitHub, звіряє версію, а перед встановленням перевіряє розмір і SHA-256 завантаженого файлу.
</details>

---

<div align="center">

Цей репозиторій містить **сторінку проєкту й релізи**. Вихідний код закритий.

**[Сайт](https://gitkalenyuk.github.io/cartelcode/)** · **[Релізи](https://github.com/gitkalenyuk/cartelcode/releases)** · **[Канал](https://t.me/YT_cartell)** · **[Чат](https://t.me/+Ovf7rTg8ClBkOGQy)**

</div>
