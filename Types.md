Types
===

Color
---
A color consists of:  

- R (Range: 0 - 255)  
- G (Range: 0 - 255)  
- B (Range: 0 - 255)  
- A (Range: 0 - 255)

The color object also provides static functions to create instance of the color object which are CSS 2.1 compatible colors:

- Black
- White
- Blue
- Yellow
- etc.

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

If the programming language that supports static typing, an implementation of vector types could look like this:

	class Vector2i //< A two-dimensional (X, Y) vector for integer values
	class Vector2f //< A two-dimensional (X, Y) vector for float values
	class Vector3i //< A three-dimensional (X, Y, Z) vector for integer values
	class Vector3f //< A three-dimensional (X, Y, Z) vector for float values

Size
---

- W (The width of the size object)
- H (The height of the size object)

A size instance behaves like a rect, but without the X- and Y-position.