# Replicator 2X profiles for Cura

**NOTE**: I haven't used these in a while - I switched to using PrusaSlicer with
my Replicator 2X, in conjunction with
<https://github.com/rpavlik/Rep2x-GCodeSnippets-PrusaSlicer>

However, you're welcome to use and contribute to these. Additionally, you might
like the start/end GCODE from that repo, which should just need some minor
adaptations to use in Cura.

## About

This started as just a copy/backup of my
`%USERPROFILE%/AppData/Local/Cura/<ver>/...` files from a Windows install of
Cura. Apparently Cura doesn't like it when you do that, since it ends up making
warnings, etc.

In any case, you can at least use the machine and extruder info.

Requires the X3GWriter plugin!

Not sure if this supports working tethered over USB, or if you have to use an SD
card. SD card works the best in any case.

Install this with Cura not running, or it might not work right.

## Installing machine/extruder definitions

You'll copy these two directories, merging them with existing directories of
the same name, to add the MakerBot Replicator 2X.

- `definitions`
- `extruders`

The destination directory differs by platform. In the paths below, change 4.5 to
the Cura version you're using:

- Windows: `%USERPROFILE%\AppData\Local\Cura\4.5\` I think... (note that appdata
  is a hidden directory, you may need to type it in the address bar)
- Linux: `$HOME/.local/share/cura/4.5`
- macOS: Sorry, no idea - Maybe under Library in your user dir?

## Installing configs

This can be a little unreliable: it may be better to just go through the "add
machine" wizard once you've installed the machine and extruder defs, then look
at the files in `quality` with a text editor to see my basic changes.

But, if you try doing it, copy these directories to the same directory as above:

- `definition_changes`
- `machine_instances`
- `quality`

## License

Do whatever you want with them, they're just settings.

Let's call it CC0-1.0. If that doesn't work for you, let me know.
