Asset Management
===

All assets needed for running the application should be managed by an asset system. This asset system should provide
the following:
* A mechanism for getting the correct file or path inside of the asset directory structure
  (Needs to handle cross-platform paths for example)
* A mechanism for getting any asset 

An examplary setup might be:
``
/
|- assets
   |- images
   |- sounds
   |- data
|- src
``
