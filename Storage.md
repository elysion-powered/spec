Storage
=======

This object provides a Local-Storage-like mechanism for writing and reading small chunks of data. The Storage
object manages the data for you, the developer can only specify a key and value to write data and a key to read
from.

Like LocalStorage, this mechanic should not be used for writing massive chunks data, just for simple operations like
writing/reading configuration files and small save files.
