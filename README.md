# Borderless Game Resolution Changer

Launch a borderless game with resolution of choice.
This works by setting your display resolution to desired resolution before launching the game
and sets it back to your current resolution after quitting the game to desktop.

Optionally you can decide to turn windows explorer off (minor performance boost).
This works by killing the windows file explorer process
and makes the file explorer is restarted after quitting the game to desktop.

## Usage

I recommend you download just the script and put it in your game folder

Set resolution to 1920 * 1080 with windows file explorer turned off.

```powershell
.\launch_game.ps1 -game_executable .\path\to\game.exe  -x 1920 -y 1080 -TurnOffExplorer
```

Set resolution to 1280 * 720 with windows file explorer turned on.

```powershell
.\launch_game.ps1 -game_executable .\path\to\game.exe  -x 1280 -y 720
```

This script also supports positional parameters.

Set resolution to 1920 * 1080 with windows file explorer turned off.

```powershell
.\launch_game.ps1 .\path\to\game.exe 1920 1080 -TurnOffExplorer
```
