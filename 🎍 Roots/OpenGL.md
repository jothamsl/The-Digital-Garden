# OpenGL

OpenGL is an API which provides us with a large set of functions that can be used to manipulate graphics and images. In itself, it's not an API, but merely a specification, developed and mainatained by the [KhronosGroup](http://www.khronos.org/). 

## Core-profile vs Immediate mode
OpenGl's immediate mode (often referred to as the **fixed function pipeline**) was a previous version which was easy-to-use for drawing graphics. The caveat was the lack of how much control developers had over how the API performed its calculations. This mode is really easy to use and understand but is  extremely inefficient. The core-profile mode forces us to use modern practices. The advantage of learning the moder approach is that it's very flexible and efficient. However, it's also more difficult to learn. When ever we try to use one of OpenGL's deprecated functions, OpenGL raises and error and stops drawing.

TODO: EXTENSIONS, STATE MACHINE, OBJECTS
