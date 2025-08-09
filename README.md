# Extra Song Credits

This mod allows you to credit more contributors of a song in base game's the pause menu with ease!

## How To Use

- Use [merge logic](https://funkincrew.github.io/funkin-modding-docs/10-appending-and-merging-files/10-02-merging-files.html#merging-into-json-files) to add your own song credits, `_merge/data/extraSongCredits.json`.
Here's a quick snippet
```json
[
  {"op": "add", "path": "/songs/-", "value": {"songName": "High (HQ)", "credits": {"Ripper": "Sam + berg8793"}}}
]
```


## A Couple Of Things To Keep In Mind

- `songName` is the song's in-game title to account for variations of the same song (i.e. Pico and Pico (Pico mix)). It does however support songID.
- There's no limit to the credits field, you can add as many as you want.
