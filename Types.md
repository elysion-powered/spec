Types
===

Color
---
A color consists of:  

- R (Range: 0 - 255 | Default value: 0)  
- G (Range: 0 - 255 | Default value: 0)  
- B (Range: 0 - 255 | Default value: 0)  
- A (Range: 0 - 255 | Default value: 255)

The color object also provides static functions to create instance of the color object which are CSS 2.1 compatible colors:

- Black
- White
- Blue
- Yellow
- etc.

An instance of color is set to have the following functions:

- `toString`: Converts the color object into a CSS color compatible rgb/rgba - string. If the alpha value is different than 255, it will be written as `alpha / 255`. For example a color object with r: 255, g: 255, b: 0 will return `rgb(255, 255, 0)`, whereas a color object with r: 255, g: 255, b: 0, a: 128 will return `rgba(255, 255, 0, 0.5)` 
- `toHex`: Converts the color object into a hex color string (e.g. `#ffffff`) while ignoring the alpha value
- `lighten`
- `darken`
- `fadeIn`
- `fadeOut`

Rect
---

- X (The X position of the rectangle)
- Y (The Y position of the rectangle)
- W (The width of the rectangle)
- H (The height of the rectangle)

A Rect instance also has to has the following functions:

- `contains`: Checks if this rect contains another rect or vector
- `center`: Returns a vector with the X- and Y-position being the center of the rect
- Arithmetic functions: Arithmetic function can either be implemented through operator overloading if the programming language supports it or through seperate functions:
	- `add`
	- `subtract`
	- `multiply`
	- `divide`

Vector
---

It is recommended, although not required to have classes for each a two-dimensional and a three-dimensional vector.
If the programming language that supports static typing, an implementation of vector types could look like this:

	class Vector2i //< A two-dimensional (X, Y) vector for integer values
	class Vector2f //< A two-dimensional (X, Y) vector for float values
	class Vector3i //< A three-dimensional (X, Y, Z) vector for integer values
	class Vector3f //< A three-dimensional (X, Y, Z) vector for float values

A vector instance has to implement these functions:

- Arithmetic functions: Arithmetic function can either be implemented through operator overloading if the programming language supports it or through seperate functions:
	- `add`
	- `subtract`
	- `multiply`
	- `divide`

Size
---

- W (The width of the size object)
- H (The height of the size object)

A size instance behaves like a rect, but without the X- and Y-position.
