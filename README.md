# Windows11-Clone

A Windows 11 desktop experience recreated in the browser using **pure HTML, CSS and JavaScript** — no frameworks, no build step, no bundlers.

**[Live demo](https://codewithsaurabhyadav.github.io/Windows11-Clone)**

Inspired by [blueedge Windows 11 (React)](https://win11.blueedge.me).

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## About

This project is a front-end-only clone of the Windows 11 experience, from the power-on animation to the lock screen, sign-in and desktop. Everything is plain HTML, CSS and vanilla JavaScript, so it runs in any modern browser with nothing to install.

## Features

### Boot and sign-in
- Power-on animation video followed by the Windows startup sound
- Lock screen with live time and date; click to reveal the sign-in screen
- Sign-in button plays a welcome video, then loads the desktop

### Desktop
- Desktop icons: This PC, Recycle Bin, Google Chrome, Epic Games, Xbox, Spotify, folders, VS Code and a GitHub shortcut
- Double-click the GitHub icon to open the author's GitHub profile
- Custom right-click context menu with View, Sort by, Refresh, New, Display Settings, Personalize and Terminal entries
- Hide or show desktop icons and refresh from the context menu
- Welcome confirmation pop-up on load; declining it goes to a separate "disagree" page

### Start menu
- Opens from the Start button on the taskbar
- Search box, pinned apps grid (Chrome, Clock, Settings, MS Office apps, Notepad, Paint, Spotify, VS Code, Xbox and more), Recommended section
- User profile and power button in the footer

### Taskbar
- Centered Windows 11 style icon layout
- Weather-style widget on the left with a day/night icon based on the current time
- Hovering the widget opens a widgets panel with a search bar and an image grid
- System tray with language, wifi, volume and battery icons
- Live clock and date

## Project structure

```
Windows11-Clone/
├── index.html          # Power-on, lock screen and sign-in
├── home.html           # Desktop, start menu, taskbar and widgets
├── disagree.html       # Page shown if the welcome pop-up is declined
├── src/
│   ├── CSS/            # style.css (lock screen), home.css (desktop)
│   └── JavaScript/     # script.js (boot/sign-in), home.js (desktop logic)
├── images/             # Desktop, taskbar, start menu and control panel icons
├── audio/              # Startup sound
└── videos/             # Power-on and welcome videos
```

## Getting started

No dependencies or build step are needed.

```bash
git clone https://github.com/itsSauraj/Windows11-Clone.git
cd Windows11-Clone
```

Then either open `index.html` in your browser, or serve the folder locally (recommended, since some browsers restrict autoplay of audio and video on `file://` pages):

```bash
# Python 3
python -m http.server 8000
# then visit http://localhost:8000
```

Start from `index.html`; it leads into `home.html` after sign-in.

> **Note:** The icon set (Font Awesome kit) and the widgets panel images (picsum.photos) are loaded from the internet, so an internet connection is needed for those to appear.

## Tech stack

- **HTML5** for structure
- **CSS3** for layout, animations and styling
- **Vanilla JavaScript** for interactivity, clock, menus and screen transitions

## Status

This is a visual clone, so many menu items and apps (Settings, Paint, Office apps and similar) are UI only and do not open real applications yet.

## Author

Made by **Saurabh Yadav** — [GitHub](https://www.github.com/codewithsaurabhyadav)

For further details please contact me.
