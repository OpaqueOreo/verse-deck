# Verse Deck Companion

The companion app for the **Verse Deck** widget on the CORSAIR XENEON EDGE: a touch cockpit for Star Citizen.

The widget can't press keys or read the game by itself. This small app runs on the same PC and does both: it reads
Star Citizen's game log so the panel follows what you're doing, and presses keys when you tap the widget.

Fan-made; not affiliated with Cloud Imperium Games.

## Download

**[VerseDeckCompanion.exe](../../releases/latest/download/VerseDeckCompanion.exe)** (from the [latest release](../../releases/latest)). No Python or other software needed.

## Install

1. Run **VerseDeckCompanion.exe**. It installs for your Windows user only, with no admin rights:
   - a Start Menu entry (Verse Deck > Verse Deck Companion)
   - an uninstaller under Settings > Apps > Installed apps
   - optionally, start with Windows

   Windows may show "Windows protected your PC" because the app isn't code-signed. Choose **More info > Run anyway**.
2. Follow the setup it opens with:
   - **Star Citizen:** it finds your install, or asks for the folder.
   - **Keybind file:** it offers to copy the Verse Deck keybinds into the game. They add keys for controls
     Star Citizen ships without one, using only keys that are free in the current patch and your profile.
     Then in game: **Options > Keybindings > Control Profiles**, import **Verse Deck** (keyboard only).
   - **Pairing code:** it shows a code for the widget.
3. In iCUE (5.52 or later), add the Verse Deck widget to a **Large or XL** slot on the XENEON EDGE.
   - Open its settings and enter the pairing code under **Companion**.
   - Allow `127.0.0.1:48765` and `api.uexcorp.space` when iCUE asks.

   Until everything is ready, the widget shows a checklist that ticks itself off.

Keep the companion running while you play: its window, or start it with Windows.

## Try it without the game

Start Menu > Verse Deck > **Verse Deck Companion (test mode)** plays a pretend session, so you can try every
part of the widget. Nothing is sent to the game.

## Good to know

- **Key presses:** it only presses keys from your taps on the widget, and only while Star Citizen is the active
  window. Anything risky (eject, self destruct) needs a deliberate hold.
- **This PC only:** it talks to the widget on this PC only, and every request needs your pairing code.
- **Settings:** your settings live in `%LOCALAPPDATA%\VerseDeck`. Run setup again with `VerseDeckCompanion.exe --setup`.
- **Uninstall:** Settings > Apps > Installed apps > Verse Deck Companion. It asks before deleting your settings.
- **Your responsibility:** one tap sends one key or key combination, like a macro pad. Using input tools with
  Star Citizen is your responsibility under the game's terms.
