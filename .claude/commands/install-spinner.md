Read the `spinners.json` file from the root of this repository. Then read the user's `~/.claude/settings.json` file.

Format of `spinners.json`:

```json
{
  "spinnerVerbs": {
    "mode": "replace",
    "verbs": ["Phrase 1", "Phrase 2"]
  }
}
```

Copy the `spinnerVerbs` field from `spinners.json` into `~/.claude/settings.json`. If the `spinnerVerbs` field already exists in `settings.json`, replace its value. If it doesn't exist, create it.

IMPORTANT: Do not modify any other fields in `settings.json`. Only change `spinnerVerbs`.
