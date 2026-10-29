
# Applications

|Type|Applications|
|---|---|
|Utils|UniGetUI, WinRAR, Free Download Manager, Revo Uninstaller, Powershell, chocolatey|
|Browser|Brave|
|Important|VLC, Sublime, Paint 3D, MS Office, Nvidia|
|Others|Powertoys/Everything, Windhawk, LocalSend, Blip, Universal x86 Tuning Utility|
|Drivers|[Ant Esport GM320 v2](https://downloads.antesports.com/get.php?type=drivers&file=ANT-GM320-GM330-GM340V2.exe)|
|YouTube|Figma, OBS, Audacity, Filmora, Subtitle Edit|
|Gaming|Steam, Epic Games, MSI Afterburner, Riva Tuna Statistics|
|Programming|VS Code, Python, Node.js, Mongo Community Server, MongoDB Compass, Unity, .NET, Git, GitHub Desktop|
|Miscallaneous|File Pilot, mp3Tag, ProtonVPN, File Converter, Free File Sync, Nilesoft Shell, Lossless Cut, Dropshelf|

# Setup

## Step 1: Basic Setup
1. Open Settings
2. Go to **Personalization > Colors**.
	- Set Choose your Mode to Dark.
	- Set Accent color according to your choice. I prefer Green color.
3. Go to **Personalization > Start**.
	- Turn off Pinned and Recent.
	- Turn on All.
	- Set Start Menu Size to Small.
	- Go to Folers, and turn off everything except Settings and File Explorer.
	- Turn off Acount Related Notifications, Recent Items in Jump List.

## Step 2: Debloat
1. Run Chris Titus Tech WinUtil and debloat Windows.
2. Uninstall Edge, One Drive, Windows Media Player, Notepad, MS Paint, Copilot and other bloat.
3. Re-install Clock, if it gets deleted.
4. Go to Regedit and fix the you see something like 'This is managed by your organization.'
	- Open regedit.
	- Go to `HKLM\SOFTWARE\Microsoft\PolicyManager\current\device\Education` and set the value of `IsEducationEnvironment` to 0.
	- Check for values such as:
		- `DisableWindowsSpotlightFeatures`
		- `ConfigureWindowsSpotlightOnLockScreen`
		- `NoChangingLockScreen`
		inside the registries like:
		- `HKLM\SOFTWARE\Policies\Microsoft\Windows\CloudContent`
		- `HKCU\SOFTWARE\Policies\Microsoft\Windows\CloudContent`
		- `HKLM\SOFTWARE\Policies\Microsoft\Windows\Personalization`
		- `HKCU\SOFTWARE\Policies\Microsoft\Windows\Personalization`
		and set these values to 0.

## Extra Steps
- Make a New template for New Empty File using Regedit.
