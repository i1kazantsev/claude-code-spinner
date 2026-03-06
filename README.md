<p align="center">
  <img src="assets/kabanchikom.png" alt="Кабанчиком" width="400">
</p>

# claude-code-spinner

Замена фраз спиннера Claude Code для уважаемых вайбкодеров.

Вместо стандартных `Thinking...`, `Analyzing...`, `Pondering...` будет крутиться **"Обкашляю вопросик"**, **"По красоте все сделаем"** и еще 90+ фраз.

## Установка через Claude Code

```bash
git clone https://github.com/i1kazantsev/claude-code-spinner.git
cd claude-code-spinner
```

Запусти Claude Code и выполни:

```
/install-spinner
```

## Ручная установка

Скопируй содержимое `spinners.json` в `~/.claude/settings.json`:

```json
{
  "spinnerVerbs": {
    "mode": "replace",
    "verbs": ["Обкашляю вопросик", "По красоте все сделаем", "..."]
  }
}
```

## Сектор приз: "Вопросик на тормозах" на хук Stop

Когда основной агент ответит, ты услышишь **«Вопросик на тормозах»**. Работает через `afplay` (уже есть на macOS).

### Установка через Claude Code

```
/install-hook
```

Если громко, попроси клод сделать потише. В ручной установке есть пример, можно `-v 1` поменять на `-v 0.5`.

### Ручная установка

Скопируй `sounds/stop-hook.mp3` в `~/.claude/sounds/` и добавь хук в `~/.claude/settings.json`:

```json
{
  "hooks": {
    "Stop": [
      {
        "matcher": "",
        "hooks": [
          {
            "type": "command",
            "command": "afplay -v 1 ~/.claude/sounds/stop-hook.mp3"
          }
        ]
      }
    ]
  }
}
```

## Лицензия

Какая еще лицензия? Ладно, MIT.

## На связи

Телега: [Несерьезный айтишник](https://t.me/neserioznoeit)<br>
Рассказываю про разработку с ИИ. Заглядывай.