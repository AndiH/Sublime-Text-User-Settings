# Sublime Text 3 User Settings
These are my user settings for [Sublime Text 3](http://www.sublimetext.com/). Based on [my Sublime Text 2 user settings](https://github.com/AndiH/st2-user-settings), plus some.

Additionally, there's

* a custom build setting for [CERN's ROOT](http://root.cern.ch/) framework,
* snippets for [CUDA Thrust](https://github.com/thrust/thrust), and
* other stuff I might find useful sharing.

## User Settings – ``Preferences.sublime-settings``
My settings are mainly based on Lars Feyerabend's. Head [over there](https://github.com/lars-feyerabend/st2-user-settings) to get an extensive explanation of each setting and some needed tools.  
Main difference: I chose a smaller font and different tab/indentation configuration.

## C++ Sublime Linter
Google's C++ style guide foresees not using tabs for indentation. But I like it. So I changed the `cpplint` behavior accordingly in the Sublime Linter user settings (`--filter=…`).

## ROOT Build Settings – ``ROOT-Shell.sublime-build``
Particle physicists love to use [CERN's ROOT](http://root.cern.ch/) framework for data analyses. Here's a small build setting which fires up `root -l` for the current file.

You probably only want to use it for syntax / error / ROOT specialty checking since most of the stuff you do in ROOT is interactive to a certain degree; Sublime Text closes the built file after a successful build, so your canvas is immediately destroyed again.

I actually don't use this build anymore.

## CUDA Thrust Snippets – ``CUDA/Thrust`
Snippets I use, which make the work with [Thrust](https://github.com/thrust/thrust) a bit faster.

Requirements: [sublime-cuda-cpp by harrism](https://github.com/harrism/sublimetext-cuda-cpp), which gives you syntax highlighting for CUDA, a build system as well as some snippets (for plain CUDA). For this, it defines a new source code language ``cuda-c++``.

## Other stuff
Just take a look.  
I was missing a snippet for ``std::cout``, so I made one.
