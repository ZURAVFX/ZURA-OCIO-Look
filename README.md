# ZURA OCIO Look

**OCIO 2 display, view and look transforms directly inside Adobe After Effects.**

ZURA OCIO Look is a Windows After Effects effect plug-in for artists who want a straightforward OpenColorIO 2 viewing transform inside a comp. Select an OCIO config, then choose the relevant **Display**, **View** and **Look** without building a separate colour-management workaround around the comp.

## What it does

The plug-in exposes an OCIO 2 display/look transform in After Effects and is designed for colour-managed CG, VFX and motion-design review workflows.

## Key features

- OpenColorIO 2 based processing
- Config-selectable OCIO display and look transform
- **Display**, **View** and **Look** controls inside the effect
- Supports external `.ocio` configuration files and the `$OCIO` environment variable workflow
- GPU rendering path with CPU/error fallback reporting
- Useful with ACES/OCIO studio or CG configurations where a reliable viewing transform is needed in After Effects

## Typical use

Use ZURA OCIO Look near the end of a viewing/review chain to preview scene-linear or managed imagery through the same OCIO display/view choices used elsewhere in a VFX pipeline. It is particularly useful when you want After Effects to match a Blender, Houdini, Nuke or Resolve OCIO viewing setup more closely.

This is a **view/look transform tool**, not a replacement for understanding the colour space of your source footage or for a correctly designed project-wide colour pipeline.

## Install — Windows

1. Download `ZURA OCIO_Look.aex` from the `dist` folder or project website.
2. Close After Effects.
3. Copy the `.aex` into an Adobe After Effects plug-ins location, for example your version's `Support Files\Plug-ins` folder or the appropriate shared Adobe MediaCore plug-in folder.
4. Relaunch After Effects.
5. Add **ZURA OCIO Look / OCIO Look Config** from the Effects menu and choose your OCIO configuration and viewing options.

## OCIO configuration

The plug-in can work with a selected OCIO configuration and recognises the standard `$OCIO` environment-variable workflow. Your available Displays, Views and Looks come from the configuration you load, so the exact menu contents depend on your pipeline config.

## Compatibility

- Current public binary: Windows `.aex`
- OpenColorIO 2 based
- Built for modern After Effects workflows

If a specific After Effects version fails to load, please open an Issue with the AE version, Windows version, GPU and OCIO config used.

## Upstream / third-party acknowledgement

This build contains OpenColorIO functionality and carries upstream references to Brendan Bolles' **AdobeOCIO** project. OpenColorIO and any upstream components retain their respective licences and copyrights. See `THIRD_PARTY_NOTICES.md`.

## Credits

Updated and packaged by **ZURA VFX** for practical motion-design and VFX colour workflows.
