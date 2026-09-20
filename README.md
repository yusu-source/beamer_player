# BeamerDeck

Минимальный статический просмотрщик PDF-презентаций для GitHub Pages и Moodle.

## Локальный запуск

```bash
python3 -m http.server 8000
```

Откройте `http://localhost:8000/?id=demo`.

## Добавление презентации

1. Положите PDF в `pdf/`.
2. Добавьте запись в `presentations.json`.
3. Откройте `https://USERNAME.github.io/beamerdeck/?id=linux-users`.

## GitHub Pages

`Settings → Pages → Build and deployment → Deploy from a branch → main → /(root)`.

## Moodle

```html
<iframe
  src="https://USERNAME.github.io/beamerdeck/?id=linux-users"
  width="100%"
  height="720"
  style="border:0"
  allowfullscreen>
</iframe>
```

Если Moodle удаляет iframe, это ограничение HTML-фильтрации/ролей на стороне Moodle.
