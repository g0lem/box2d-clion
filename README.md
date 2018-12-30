# box2d-clion

I made this so that you could easily build the Box2D library using CLion. 
Just load the CMake Project and build it.

Don't forget to link the library in your project and paste the box2d.a in your library folder 
(the one where you do ``link_directories(./lib)``)

```cmake
project(YOUR_PROJECT)
target_link_libraries(YOUR_PROJECT box2d)
```

This is also going to output a bunch of values, since it compiles an executable as well.

*(If the executable fails to compile, it means you have a problem and you won't be able
 to use the library)*

If you want to use this, you will also have to do:
```cmake
include_directories(./include)
```

where the ``./include`` folder is the one where you have the Box2D sources.