# Custom Zsh Themes & Configs

This repository contains custom configuration modifications for terminal prompt themes.

## 1. Powerlevel10k Configuration (`p10k.zsh`)
Modifications made to the standard Powerlevel10k theme to display:
` [11:20 a.m]~/iOS-Projects/custom-p10k/ [main]`

- **Time Segment Insertion**: Positioned the `time` segment in `POWERLEVEL9K_LEFT_PROMPT_ELEMENTS` right after `os_icon` and before `dir`.
- **Time Format**: Configured using `%-I:%M %p` (12-hour format, unpadded hour, e.g., `3` instead of `03`).
- **Clean Layout**: Removed the default clock icon (`POWERLEVEL9K_TIME_VISUAL_IDENTIFIER_EXPANSION=''`).
- **Bracketed Lowercase Time**: Formatted the output using `POWERLEVEL9K_TIME_CONTENT_EXPANSION` to surround it with square brackets and lowercase/dot the indicator (`[11:20 a.m]` or `[3:45 p.m]`).

## 2. Candy Zsh Theme (`candy.zsh-theme`)
Modifications made to match the single-line layout:
` [11:33:07] [~/iOS-Projects/custom-p10k] [main *]`

- **Single Line Layout**: Simplified the prompt to a single line containing ` [Time] [CWD] [Git Info]`.
- **Time Segment**: Configured inside brackets using `%D{%H:%M:%S}`.
- **Enhanced Visibility**: Upgraded the time color to a bright `Deep Sky Blue` (`%F{39}`) for improved readability on dark terminal backgrounds.
- **Directory Path**: Wrapped the directory (`%~`) inside white brackets: `[%~]`.
