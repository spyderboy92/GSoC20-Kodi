# Google Summer of Code’ 20 Wrap Up


Finally it is time for wrapping up my GSoC project. A great summer journey coming to an end. The community has been more than helpful. I couldn’t have asked for more. 


## The Idea:

Inputstream.adaptive is written in C++, and handles different streams for Kodi. 
The aim of my project was to introduce variable time-length stream buffering, and then add adaptive switching of different representations depending upon different constraints like available network bandwidth, available window resolution, computation power available, etc

## Work done:

![Rep switching](https://ibb.co/L0tsq7T)
![Screenshot IA(UI- Menu)](https://ibb.co/L0tsq7T)


Added UI control that can be segregated for noob user to advanced user depending on access  level.
Assured Buffer Duration- Tries to always maintain this buffer duration completely. 
Max Buffer Duration- The max buffer length to store. Can be configured for movie watching. This will be always filled with best quality.
Ignore Window Change- If disabled, selection of stream quality will depend on Kodi window size too.
PRs and commit for the work done:

### Changes in inputstream.adaptive:
* https://github.com/peak3d/inputstream.adaptive/pull/494
* https://github.com/peak3d/inputstream.adaptive/pull/506
* https://github.com/spyderboy92/inputstream.adaptive/commit/cbc108813d239163cfb90a80c06b9359478748c5
### Xbmc patch for Display Update:
* https://github.com/xbmc/xbmc/compare/master...spyderboy92:IA_DisplayRefresh

## Experience
It was a very thrilling summer experience. First 2 months went very great for me. Last month had some personal setbacks. Overall got to learn a lot of stuff in the journey. A wonderful community with a great mentor. Would love to become a regular contributor in future.

## In the end, a big thanks to team Kodi and Google for providing me this wonderful opportunity as a student.
