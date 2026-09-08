# Портфолио Никиты Козлова

Статическая версия сайта: HTML, CSS и изображения. Для работы ей не нужны Tilda, база данных или платный сервер.

## Как опубликовать через GitHub Pages

1. Войдите на [github.com](https://github.com/) и создайте новый публичный репозиторий, например `kozlov-portfolio`.
2. Откройте репозиторий и нажмите **Add file → Upload files**.
3. Перетащите в окно всё содержимое этой папки: `index.html`, `styles.css`, `README.md`, `.nojekyll` и папку `assets`.
4. Нажмите **Commit changes**.
5. Откройте **Settings → Pages**.
6. В поле **Source** выберите **Deploy from a branch**.
7. Выберите ветку **main**, папку **/(root)** и нажмите **Save**.

Через несколько минут сайт откроется по адресу вида:

`https://ВАШ-ЛОГИН.github.io/kozlov-portfolio/`

Официальная инструкция: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Как подключить kozlov-na.ru

Сначала откройте **Settings → Pages**, укажите `kozlov-na.ru` в поле **Custom domain** и сохраните. Только после этого меняйте DNS в REG.RU.

Для корневого домена добавьте четыре A-записи:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Для `www` можно добавить CNAME-запись на `ВАШ-ЛОГИН.github.io`.

Не удаляйте MX- и TXT-записи, если они используются почтой. Обновление DNS может занять до 24 часов. После подключения включите **Enforce HTTPS** в настройках GitHub Pages.

Официальная инструкция: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Как изменить сайт без специальных программ

Файлы можно редактировать прямо на GitHub. VS Code понадобится только в том случае, если вы захотите работать с кодом на своём компьютере.
