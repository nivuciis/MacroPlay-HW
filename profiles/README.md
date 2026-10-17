# Profiles

Each profile is a JSON file with a name, a color, the 12 keys and the 3 encoder actions.

```json
{
  "name": "Blender",
  "color": "#F5792A",
  "keys": {
    "1": { "label": "Front", "on_press": [{ "type": "key", "keys": ["KEYPAD_ONE"] }], "on_release": [] }
  },
  "encoder": {
    "clockwise":        [{ "type": "key", "keys": ["RIGHT_ARROW"] }],
    "counterclockwise": [{ "type": "key", "keys": ["LEFT_ARROW"] }],
    "click":            [{ "type": "key", "keys": ["SPACE"] }]
  }
}
```

The final format will be frozen at the end of Phase 1 of the roadmap. Until then, it may change.

## Rules for online game profiles

One key, one action. No automatic sequences, repetition or delays in profiles marked as online games.
