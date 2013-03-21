Texture
---

It in its core, a texture is basically a behaviour which attached to a entity may provide its graphical representation.

A texture needs the following functions:
* loadFromFile
* pixels[x][y] <-- provides read access to any pixel of the texture
* width
* height

As soon as the texture is loaded, the pixels are written to the array which then can be accessed.
