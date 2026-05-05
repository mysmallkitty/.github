# My Small Kitty

![logo](https://raw.githubusercontent.com/mysmallkitty/my_small_kitty/refs/heads/main/graphics/ui/logo.png)

**My Small Kitty** is a 2D platformer game built with Godot.

The project includes a playable platformer client, an in-game map editor, user-created map upload/download features, online rankings, replay data, and ghost features connected to a FastAPI backend.

---

## ScreenShots

![Gameplay1](https://img.itch.zone/aW1nLzI1NDI4NzUyLmdpZg==/original/GPZAMO.gif)
![Gameplay2](https://img.itch.zone/aW1nLzI1NDI4ODE1LmdpZg==/original/fCEYbn.gif)
![Editor1](https://img.itch.zone/aW1nLzI1NDI5MTI4LmdpZg==/original/0IRMUh.gif)

---

## Links

- Itch.io: https://h4yase.itch.io/mysmallkitty

---

## Overview

My Small Kitty is structured as a client-server game project.

The Godot client handles gameplay, map editing, local play data, replay playback, and UI.  
The FastAPI server handles accounts, map data, rankings, replay metadata, and online features.

```text
Godot Client
    |
    | HTTP / WebSocket
    v
FastAPI Server
    |
    |-- PostgreSQL
    |-- Redis
