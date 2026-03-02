<p align="center">
  <img src="assets/kabanchikom.png" alt="Кабанчиком" width="400">
</p>

# claude-code-spinner

Замена фраз спиннера Claude Code для уважаемых вайбкодеров.

Вместо стандартных `Thinking...`, `Analyzing...`, `Pondering...` будет крутиться **"Обкашляю вопросик"**, **"По красоте все сделаем"** и еще 70+ фраз.

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

## Лицензия

Какая еще лицензия? Ладно, MIT.
