# Stories on the Stone

Інтерактивний урок англійської (B1, 90 хвилин) для Насті й Андрія: наскельне мистецтво Австралії, лексика світових загадок, неформальний лист. Одна статична сторінка без збирання та залежностей.

## Файли

- `index.html`: увесь урок (HTML, CSS і JS в одному файлі)
- `vercel.json`: налаштування Vercel (чисті URL, заголовки, `noindex`)
- `.gitignore`: службові файли, які не потрібно публікувати

## Як опублікувати

### 1. GitHub (через браузер, без Git)

1. Відкрий github.com → **New repository**.
2. Назва: `stories-on-the-stone`. Видимість: **Private** (щоб не був публічним).
3. Натисни **Create repository**, потім **uploading an existing file**.
4. Перетягни всі файли з цієї папки (`index.html`, `vercel.json`, `.gitignore`, `README.md`).
5. Натисни **Commit changes**.

### 1б. GitHub (через Git на Windows)

```bash
cd stories-on-the-stone
git init
git add .
git commit -m "Stories on the Stone: first version"
git branch -M main
git remote add origin https://github.com/<твій-логін>/stories-on-the-stone.git
git push -u origin main
```

### 2. Vercel

1. Відкрий vercel.com → **Add New… → Project**.
2. Вибери репозиторій `stories-on-the-stone` → **Import**.
3. Нічого не змінюй: Framework Preset = **Other**, Build Command і Output Directory порожні.
4. Натисни **Deploy**. За хвилину буде адреса `https://stories-on-the-stone.vercel.app`.

Кожен наступний `git push` (або заміна `index.html` на GitHub) автоматично оновлює сайт.

## Як оновлювати урок

Замінити `index.html` новою версією (на GitHub: відкрити файл → значок олівця або **Add file → Upload files**) і зробити Commit. Vercel сам передеплоїть сторінку.

## Примітки

- Прогрес учня зберігається лише в пам'яті сторінки; чернетка листа та плану зберігається в браузері учня (`localStorage`).
- Шрифти (Lora, Onest, JetBrains Mono) підвантажуються з Google Fonts. Без інтернету працює запасний набір шрифтів.
- Сторінка має `noindex`, тому в пошуку Google не з'явиться. Хто має посилання, той її відкриє. Якщо потрібен пароль, увімкни **Settings → Deployment Protection** у Vercel.
