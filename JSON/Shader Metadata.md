# `name`

Type: String

Name of the shader. Shown in the options menu, so it should be kept short.


# `downscaling`

Type: Boolean

Whether the framebuffer should be downscaled before being supplied to the
shader. This is useful for shaders that wish to sample the framebuffer at a low
resolution, like the CRT shader does.

The exact resolution to downsample to is determined by `pixel_alignment_shift`
(see `Setting.md` for more information).
