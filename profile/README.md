# My Small Kitty

**My Small Kitty** is a 2D platformer game built with Godot.

The project includes a playable platformer client, an in-game map editor, user-created map upload/download features, online rankings, replay data, and ghost features connected to a FastAPI backend.

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
