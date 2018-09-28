---
layout: page
title: Mojito
---

Fishing Cactus cross platform game engine (C++) running on 3DS, Android, HTML5, iOS, Linux, macOS, PS3, PSP, Samsung Bada, Wii, Windows, and Xbox360.

Features
* Entity-Component system
* Lua and JS scripting
* HTML-based UI
* Post processes and scriptable render passes
* Cross platform asset building toolchain (with auto detected dependencies)
* Animation blend tree
* Asset streaming
* Asset and scripts hot reload
* Web tools for inspection and profiling
* Cross-platform configurable project generation and build system with dependencies/package manager (based on premake + ant + ivy + jenkins + reviewboard, reviewable.io + builder2 + unit tests)
* Audio with OpenAL, FMOD and XAudio backends
* ...

Features
* multiplatform
  * win
  * macos
  * linux
  * ios
  * android
  * winphone
  * 3ds
  * wii
  * samsung bada
  * xbox360
  * ps3 (WIP)
* graphics
  * async loading
  * small objects (TEXTURE_2D)
  * dae
  * materials
  * skinning
  * lights
  * cinematics
  * shadows
    * cascaded shadow maps
    * dynamic lighting
  * directional
  * point
  * spot
  * scriptable render pipeline
  * visible sets
  * fragments
  * inputs and outputs FB
  * forward renderer
  * light prepass renderer
  * full deferred
  * multi APIs
  * animation blend tree
* UI
  * home made
  * librocket
  * gameswf
  * litehtml
* materials and effects
  * effect like system for glsl (xml with includes and defines)
  * 3ds shaders
  * shadershaker / fragments
* render thread
* condition variable to trigger resource creation / rendering
* queued rendering WIP
* particles
  * particle universe
  * simulated continuous emission
Light probes
* kernel
  * allocators
  * reflection / serialization (binary, byteswapping, json)
  * modern c++ features
    * move operator
    * typelists
    * string_view / array_view
    * future / promise
* network file system
* Net
  * socket.io
* AWS
  * cognito
  * lambdas
  * mongodb
  * SNS
  * ...
* audio
  * openAL
  * xaudio
  * fmod
* libs
  * bullet
  * recast/detour
* gameplay

* debug
  * embedded web server (using mongoose)
  * probe institute
  * perf graphs
  * parameter tweaking + save to xml
  * 'blend graph'
  * heap inspector
  * pix events
  * potential deadlock detection

* resource compiler
  * vertex cache optim
  * texture compression
  * dependency manager
  * sqlite
  * lod0
  * static batching
    * atlas creation

* scripting
  * lua

* input
  * kinect
  * dtw
  * consensus