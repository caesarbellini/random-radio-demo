# Random Radio

A single-page radio that plays truly random songs. No algorithm, no curated playlists: every track is picked at random from the [Deezer](https://developers.deezer.com/api) catalog, with [MusicBrainz](https://musicbrainz.org/doc/MusicBrainz_API) used for genre and year filters.

**Live demo:** https://caesarbellini.github.io/random-radio-demo/

## Features

- Pure randomness by default; every filter is off until you turn it on
- Optional filters: source, popularity (minimum or range), release years, genre (search ~2,200 genres, random genre, rotate every N songs), explicit
- Similar mode, based on the current artist
- Tap a genre badge to mix 3 songs of it into Up next, make it your radio, or learn about it
- Crossfades, loudness leveling, preloading, history, favorites, artist and album sheets
- Liquid-glass UI that works on desktop and mobile

## Run locally

It is a single HTML file with no build step:

```sh
python3 -m http.server 8000
# open http://localhost:8000/random_radio.html
```

Audio comes from Deezer's 30-second previews.
