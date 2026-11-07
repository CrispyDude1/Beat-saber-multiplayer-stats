# Beat Saber Multiplayer Player Info

<img width="881" height="449" alt="Screenshot 2026-11-07 141807" src="https://github.com/user-attachments/assets/d4b6a6f9-f77f-465f-81a7-40d970ac3b06" />

A Beat Saber multiplayer mod that displays additional player profile information directly above each player's head while they're in the multiplayer lobby.

The mod combines **ScoreSaber** and **BeatLeader** information into one convenient panel, allowing you to see other players' stats, rankings, and profile details without having to look them up manually.

## Features

- **Multiplayer Player Panels** – Displays an information panel above each player's head in the multiplayer lobby.
- **ScoreSaber Integration** – Retrieves and displays each player's ScoreSaber profile information.
- **BeatLeader Integration** – Retrieves and displays each player's BeatLeader profile information.
- **Automatic Player Detection** – Attaches the correct information panel to each player and follows them as they move around the lobby.
- **Automatic Profile Updates** – Refreshes player information after multiplayer songs finish and players return to the lobby.
- **Platform Images** – Displays platform-specific images for ScoreSaber and BeatLeader.
- **In-Game Settings Menu** – Includes its own settings page in the Beat Saber Mods Tab
.

## Information Displayed

Each player has a panel containing two separate sections: ScoreSaber and BeatLeader.

### ScoreSaber

Displays the player's ScoreSaber information, including:

- **PP** – The player's total performance points.
- **Global Rank** – Their worldwide ScoreSaber ranking.
- **Country Rank** – Their ranking within their country.
- **Headset** – The headset information available on their profile.
- **Platform** – The platform they're playing on, such as PC Steam.
- **Profile Picture** – Their ScoreSaber profile picture.

### BeatLeader

Displays the player's BeatLeader information, including:

- **PP** – The player's total BeatLeader performance points.
- **Global Rank** – Their worldwide BeatLeader ranking.
- **Country Rank** – Their ranking within their country.
- **Level** – Their current BeatLeader level.
- **Prestige** – Their current prestige.
- **XP Progress** – Their current XP progress toward the next level, displayed in a format such as `790/10000 XP`.
- **Headset** – The headset information available on their profile.
- **Platform** – The platform they're playing on, such as PC Steam.
- **Profile Picture** – Their BeatLeader profile picture.

ScoreSaber and BeatLeader information are displayed separately so players can easily compare both platforms.

## In-Game Settings

The mod includes its own settings page inside the Beat Saber **Mods** menu.

### Transparent Background

<img width="891" height="473" alt="Screenshot 2026-11-07 141641" src="https://github.com/user-attachments/assets/8e2901fc-6b04-4f37-8b43-8b63b4eb93df" />


Players can enable or disable the panel's background transparency using the **Transparent Background** toggle.

- **Enabled:** Makes the panel background fully transparent.
- **Disabled:** Restores the normal panel background.

Changing this setting only affects the background. All text, player information, profile pictures, and platform images remain visible.

The setting is saved, so your preference is retained when you restart the game. Changes also apply to existing panels and newly detected players.

## Automatic Information Refresh

Player information is refreshed automatically after a multiplayer song finishes and everyone returns to the lobby.

The mod waits approximately 10 seconds before refreshing information such as:

- ScoreSaber PP and rankings.
- BeatLeader PP and rankings.
- BeatLeader Level and Prestige.
- BeatLeader XP progress.
- Other available profile information.

Existing panels are updated instead of creating duplicate panels.

The mod also uses caching to avoid unnecessary repeated requests. If information cannot be retrieved, it can retain previously loaded information and retry when appropriate.

## Lobby Visibility

The player information panels are designed for the multiplayer lobby.

- Panels are visible while players are in the lobby.
- Panels are hidden when a multiplayer song begins.
- Panels remain hidden during active gameplay and spectator viewing.
- Panels return when players finish the song and return to the lobby.

This keeps the panels from interfering with gameplay or cluttering the spectator view.

## Player Tracking and Panel Placement

Each information panel is attached to its corresponding player and follows their movement in the lobby.

Panels are positioned above players' heads, with consideration for the existing player nameplate and ping display. The intention is to keep the information readable without overlapping other multiplayer UI elements.
