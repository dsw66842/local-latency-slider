I took blue-dev's code for the [orginal arena latency slider mod](https://github.com/blu-dev/arena-latency-slider) and modified it so that it only works with local online. You can see the readme on the original repo to get details as to how exactly the mod works.

## Installation

1) ~~Make sure you have [skyline](https://github.com/skyline-dev/skyline/releases) installed.~~
(Skyline currently has an issue with LAN/LDN, so check the troubleshooting section below for a workaround for this step)

2) Download the latest `liblocal_latency_slider.nro` from the releases page.
Place it in the corresponding folder. This is how it should look:
```
Yuzu:
%yuzu_folder%/sdmc/atmosphere/contents/01006A800016E000/romfs/skyline/plugins/liblocal_latency_slider.nro

Ryujinx:
%ryujinx_folder%/sdcard/atmosphere/contents/01006A800016E000/romfs/skyline/plugins/liblocal_latency_slider.nro
```


## Usage

When your in the local online menu or in the character select screen (for local online), you can press DPAD left/right to adjust the delay.

Ideally you would want to use this on an emulator like yuzu and combine it with the 120 fps mod. This will give you very close to native delay when playing online on LDN.


## Troubleshooting

Currently there is an issue with skyline not allowing us to go into the local wireless menu. This requires a workaround:

Yuzu Workaround:
1) Download this online fix: https://drive.google.com/file/d/1NX8Cbhax3vafTPUpp7r401oZea-Wtmi5/view
2) Place the files in `%yuzu_folder%/sdmc/atmosphere/contents/01006A800016E000/exefs/`
3) Open yuzu but DONT connect to yuzu LDN yet. First start smash.
4) Once your in the smash main menu you can connect to yuzu LDN. It'll give you a warning that the game is already running which you can ignore.
5) Open the local wireless menu and play.

Ryujinx Workaround:
1) Download this online fix: https://drive.google.com/file/d/1NX8Cbhax3vafTPUpp7r401oZea-Wtmi5/view
2) Place the files in `%ryujinx_folder%/sdcard/atmosphere/contents/01006A800016E000/exefs/`
3) Open Ryujinx (LDN version) and start smash. You should be able to go to the local wireless menu now.

