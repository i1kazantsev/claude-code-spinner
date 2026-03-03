Read the `hooks.json` file from the root of this repository. Then read the user's `~/.claude/settings.json` file.

Format of `hooks.json`:

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

Steps:

1. Create the directory `~/.claude/sounds/` if it doesn't exist (use `mkdir -p`).
2. Copy the sound file `sounds/stop-hook.mp3` from this repository to `~/.claude/sounds/stop-hook.mp3`.
3. Merge the `hooks` field from `hooks.json` into `~/.claude/settings.json`. If a `hooks` field already exists in `settings.json`, replace its value. If it doesn't exist, create it.

IMPORTANT: Do not modify any other fields in `settings.json`. Only change `hooks`.
