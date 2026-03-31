# Extra Song Credits

This mod lets you add more contributors of a song in base game's pause menu with ease!

## How To Use

- Use a [JSON patch file](https://thekade.net/funkin-cookbook/category/introduction/05.appendingandmerge.html) to add your own song credits without breaking compatibility with other mods with the path being.
Here's a quick snippet
```json
[
  {"op": "add", "path": "/songs/-", "value": {"songName": "High (HQ)", "credits": {"Ripper": "Sam + berg8793"}}}
]
```
The file should be in `_merge/data/extraSongCredits.json`

## A Couple Of Things To Keep In Mind

- `songName` is the song's in-game title to account for variations of the same song (i.e. Pico and Pico (Pico mix)). It does however support songID or internal song names (in case of two mods having the same song title).
- There's no limit to the credits field, you can add as many as you want.
