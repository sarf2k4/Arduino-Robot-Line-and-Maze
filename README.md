# Arduino-Robot-Line-and-Maze
##INTRO
-This is a code for Arduino Robot that has Line and Maze mode in one sketch

##KNOWN ISSUES
- v1.2 onwards has problems where the Maze mode codes disrupts the Line Mode making the robot unable to follow the line properly when it's still in Line Mode
- Only v1.4 are tested without any logics to make the robot do a 90 degree turn on junctions/corners 
- Without the turn logics, the robot unable do 90 degree elbow turn properly but it will stay dead center

##CHANGELOGS
###v1.5
- Enforced Mode switching to be more stricter
- Added logic on Maze mode
- Turn left are prioritized 
- Used Timer Library from https://github.com/JChristensen/Timer to avoid robot turning when detected small hole
 
###v1.4
- Added " IF (0)" block to quickly disable turn on Maze Mode
- Added new line follow (linef2()) function with PID from arduino LineFollow.cpp library as experimental

###v1.3
- Changed the condition to change to Maze Mode slightly stricter
- Still got bugs

###v1.2
- Added Maze Mode code
- Maze Mode uses separate PID from WIKIPEDIA pesudo 
- Maze Mode uses left wall follow mode
- some hitches with Maze Mode disrupting Line Mode (unable to follow line properly)
- Added automatic mode change from Line Mode to Maze Mode with basic conditions

###V0.5
- Added Speed multiplier based on percentage

###V0.1
- Basic line follow codes 
- No PID controls
