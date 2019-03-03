# lightbox
TCL embedded rehash of fluxbox in C as compositing window manager.

# What is this?
Fork of Fluxbox (with the C++ bits converted to Modular C) combining
slowly with compton to provide an in-process compositor.

# Why take the time to port fluxbox to C?
Becuase I despise the overhead of C++ on my time and want the ability to 
focus on the finer bits. Embedding a TCL Interpreter in C is much simpler 
than c++. After I have a working prototype, I intend on making this
extensable in many ways... through a linkable library, TCL Module, or TCL
Scripts, all of these again are simpler in C from my perspective.

# Purpose
Build a simple unified compositing window manager on top of the compton 
fork by Bernd Busse[tryone144]. Provide OpenGL Filter interface to allow 
creation of filters from an abstract API. Refactor fluxbox in C and overlay 
it on top of compton to provide better interaction between the window 
manager and the features provided by compton.

# Todo:

  * Embed TCL Interpreter
  * Port screen, window, menu, and keys for base functioning compositing
    window manager.
  * Provide a socket/control interface to control a running instance of wm.
  * Extend XEvents into TCL.
  * Expose OpenGL Shaders, window transformation, and filters to TCL.
