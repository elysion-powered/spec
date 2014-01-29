Asset Management
===

All assets needed for running the application should be managed by an asset system. This asset system should provide
the following:
* A mechanism for getting the correct file or path inside of the asset directory structure
  (Needs to handle cross-platform paths for example)
* A mechanism for getting any asset and returning an instance of the specific asset

An examplary setup might be:
```
/  
|- assets  
   |- images  
   |- sounds  
   |- data  
|- src  
```


Asset groups can be defined and used with conditionals, like say load full-hd images on full HD screens and lower resolutions for mobile phones.
