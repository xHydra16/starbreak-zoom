## Zoom for StarBreak (Steam edition)

### Features

- adjustable zoom during play
- borderless fullscreen

### Usage

- make sure your game is set to windowed mode
- download the .EXE from latest [release](https://github.com/atomizer/starbreak-zoom/releases/latest)
- put the executable in a separate folder, it will drop some files next to it
- on first start, you are asked to show where the game is located
- launch the game and play

### Default keys

Zoom in: Numpad +
Zoom out: Numpad -
Native resolution: Numpad 0

### Limitations

- assigned keys are always active; do not assign keys that you are going to use for something else
- does not work correctly in fullscreen mode
- there are problems with OBS in "Game capture" mode - use "window capture" for now
- might impact performance on low-end machines

### Settings

To edit the keys, window size and which monitor to put the window on, right-click the loader icon. To apply the settings you need to close and re-open the game. Acceptable key names can be found [here](https://autohotkey.com/docs/KeyList.htm).

## Creating the binary

If you don't trust me, you can compile the EXE yourself. You will need:

- installed [AutoHotkey](https://autohotkey.com/download/ahk-install.exe)
- 32bit Unicode [AutoHotkey.dll](https://github.com/HotKeyIt/ahkdll-v1-release/tree/master/Win32w)
- 32bit [MinHook.dll](http://www.codeproject.com/Articles/44326/MinHook-The-Minimalistic-x-x-API-Hooking-Libra)

Put the DLLs in root folder of the project and use the "Compile .ahk to .exe" AutoHotkey tool on `loader.ahk`, using 32 bit AutoHotkey as base executable.

Alternatively, after acquiring the DLLs, you can just run `loader.ahk` without compiling (don't forget to use 32 bit AutoHotkey).

### Credits

- Everything in `Lib/` folder and [AutoHotkey_H](https://github.com/HotKeyIt/ahkdll): [HotKeyIt](https://github.com/HotKeyIt)
- [MinHook](https://github.com/TsudaKageyu/minhook/): [TsudaKageyu](https://github.com/TsudaKageyu)

### License

MIT for my code (`loader.ahk` and `remote.ahk`); licenses for other components can be found by following the links above.