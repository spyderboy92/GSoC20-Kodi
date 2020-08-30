# Google Summer of Code’ 20 Wrap Up
![Kodi](https://user-images.githubusercontent.com/24195133/91663660-e5beb300-eb07-11ea-92cc-28c3627561ca.png)

A great summer journey coming to an end. Finally it is time for wrapping up my GSoC project. The community has been more than helpful. I couldn’t have asked for more. 


## Intro:

Inputstream.adaptive is an add-on for Kodi, written in C++, and handles different streams for Kodi. 
The aim of my project was to introduce variable time-length stream buffering, and then add adaptive switching of different representations depending upon different constraints like available network bandwidth, available window resolution, etc.


#### Basic overview of streaming mechanism
![Rep switching](https://user-images.githubusercontent.com/24195133/91663058-169ce900-eb04-11ea-8efb-c210d8d3d057.png)  
Any streaming content is basically splitted into smaller chunks called as segments.
  
  
## Work done:
* First went to work with creating buffer. It was the most difficult and learning phase. Lots of literature stuff about streaming and thread deadlocks.
* Network bandwidth based adaptive switching- It takes into account available bandwidth wrt to buffer fetching required to predict which next segment should be pre-fetched. 
* Display toggle- If the user changes Kodi window change for certain duration, new display resolution will be taken into consideration for fetching new segments.
  
  
#### Added UI option that can be segregated for noob user to advanced user depending on access level.  
![Screenshot IA(UI- Menu)](https://user-images.githubusercontent.com/24195133/91663084-42b86a00-eb04-11ea-8001-ff82df9bcb63.png)
Assured Buffer Duration- *Tries to always maintain this buffer duration completely.*   
Max Buffer Duration-     *The max buffer length to store. Can be configured for movie watching. This will be always filled with best quality.*  
Ignore Window Change-    *If disabled, selection of stream quality will depend on Kodi window size too.*  

## PRs/commit of the work:

### Changes in inputstream.adaptive:
* https://github.com/peak3d/inputstream.adaptive/pull/494
* https://github.com/peak3d/inputstream.adaptive/pull/506
* https://github.com/spyderboy92/inputstream.adaptive/commit/cbc108813d239163cfb90a80c06b9359478748c5
### Xbmc patch for Display Update:
* https://github.com/xbmc/xbmc/compare/master...spyderboy92:IA_DisplayRefresh

## Future work
Standardized resolution like HD, FHD, QHD can be made available to user, will be helpful if too many stream representations are available. This will simplify switching and will provide better user experience. 

## Experience
It was a very thrilling summer experience. First 2 months went very great for me. Last month had some personal setbacks. Overall got to learn a lot of stuff in the journey. A wonderful community with a great mentor. Would love to become a regular contributor in future.

## In the end, a big thanks to team Kodi and Google for providing me this wonderful opportunity as a student.
