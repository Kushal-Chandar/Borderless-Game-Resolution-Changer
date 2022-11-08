# Borderless Game Resolution Changer

Launch a borderless game with resolution of choice.
This works by setting your display resolution to desired resolution before launching the game
and sets it back to your current resolution after quitting the game to desktop.

Optionally you can decide to turn windows explorer off (minor performance boost).
This works by killing the windows file explorer process
and makes the file explorer is restarted after quitting the game to desktop.

## Usage

Set resolution to 1920 \* 1080, Where you display resolution is 3840 \* 2160 windows file explorer turned off.

```powershell
.\launch_game.ps1 -GameExecutablePath .\path\to\game.exe -GameWidth 1920 -GameHeight 1080 -DisplayWidth 3840 -DisplayHeight 2160 -TurnOffExplorer
```

Set resolution to 1280 \* 720, Where you display resolution is 1920 \* 1080 windows file explorer turned on.

```powershell
.\launch_game.ps1 -GameExecutablePath .\path\to\game.exe -GameWidth 1280 -GameHeight 720 -DisplayWidth 1920 -DisplayHeight 1080
```

This script also supports positional parameters.

Set resolution to 1920 \* 1080, Where you display resolution is 3840 \* 2160 windows file explorer turned off.

```powershell
.\launch_game.ps1 .\path\to\game.exe 1920 1080 3840 2160 -TurnOffExplorer
```
