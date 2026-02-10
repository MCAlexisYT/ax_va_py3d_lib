All credit goes to the creator of the parent repository (@ax_va), Lee Stemkoski and Michael Pascale. The latter two created the book *"Developing Graphics Frameworks with Python and OpenGL"*.

Here's a list of changes:
* `py3d/core/base.py`: 3 new parameters to `Base.__init__()`:
1. `additional_flags`: Additional `pygame` display flags, such as `pygame.RESIZABLE` for resizable windows. Defaults to nothing, aka 0. If you want to add more than one flag, you have to separate them with `|`.
2. `use_antialiasing`: Enables or disables anti-aliasing. Defaults to `True`, as the anti-aliasing is hard-coded into the original version.
3. `window_title`: Allows you to choose a window title that is different from the hard-coded value of `"Graphics Window"`.
* That's it.

Also, on Ubuntu, you may encounter the error `OpenGL.error.Error: Attempt to retrieve context when no valid context`.
See a bug report and suggestions to resolve it: https://github.com/pygame/pygame/issues/3110
