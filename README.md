# Playlist Chaos

## Description

An AI110 debugging exercise built around a Streamlit playlist organizer. It groups song metadata by mood and lets learners investigate intentionally inconsistent behavior. It does not play or stream music.

## Dependencies

Python 3, pip, and `streamlit>=1.36.0` from `requirements.txt`.

## Technologies

Python and Streamlit. Song data, preferences, and pick history are held in Streamlit session state.

## Setup

```bash
git clone https://github.com/bryan3342/ai110-module1tinker-playlistchaos-starter.git
cd ai110-module1tinker-playlistchaos-starter
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

On Windows, activate the environment with `.venv\Scripts\activate` instead.

## Features

- Add songs with title, artist, genre, energy, and tags.
- Configure mood thresholds and a favorite genre.
- Browse Hype, Chill, and Mixed playlists.
- Search by artist, request a lucky pick, and inspect statistics and history.
- Reset sample songs and clear history.

Known exercise issues remain in `playlist_logic.py`: search checks substring containment in the wrong direction, some statistics use only Hype songs, and random selection does not handle an empty list. The original activity asks learners to identify at least five issues, fix at least four, and check each change manually.

## Commands to run

```bash
python -m streamlit run app.py
```

No automated test suite is checked in.

## Contributors

- [Jamila Cocchiola (@jamjamgobambam)](https://github.com/jamjamgobambam), credited in the starter's Git history.

This copy is hosted by [@bryan3342](https://github.com/bryan3342). The inspected history contains no Bryan-authored implementation commits.
