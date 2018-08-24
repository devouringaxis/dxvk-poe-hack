# What?
A hack for dxvk to not stall the rendering thread when compiling shaders. This "solves" shader compilation stutter, with the downside of graphical glitches. Depends heavily on what the game does with the shaders: could work on some games fine and others will be horribly broken.

Enabled by default for Path of Exile.

### Games tested
* Path of Exile: seems fine

### Instructions

* Patch dxvk with pipeline.patch
* If trying it for other games, set dxvk.useAsyncPipeCompiler and dxvk.dontWaitForShaders to true in config
