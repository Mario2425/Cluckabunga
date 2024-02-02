# Cluckabunga
KFD Customization Tool for iOS 16.2-16.5 &
16.6b1 | Support for puaf_landa will be
available as soon as i finish. 

# In the next update
Added: Support for iOS 16.6b2-16.6.1 & 17.0b5


Added: KFD puaf_landa


NOT SURE: Possible TrollStore installer

# Download 
IPA will be available in the [releases] section as soon as i finish.


## Features
- Springboard
    - Hide dock
    - Hide home bar
    - Hide folder backgrounds

- Locks
    - Importing locks from TrollLock
    - Custom number of frames + custom animation speeds (see below)
 
- Explore
    - Find and download themes for locks and passcodes! (needs testing)
 
- Other Tools
    - Custom Fonts
    - Settings App Customizer
    - Apple Cards Changer (it broke for now)
    - Passcode Key Changer
 
## Installing
You can install through AltStore, Sideloadly,TrollStore or Xcode

## Creating Custom Lock Animations
Lock animations are very simple to make. For the frames, each image must be named "trollformation" with a number afterwards (ie. trollformation1.png, trollformation2.png, trollformation3.png...). You can use up to 120 frames, though I am not sure of the exact size limit, which is probably much less.
**If your animation is not exactly 40 frames or you want to customize the display length of each frame, you need to define the animations.** This is very simple to do:
1. Create a json file named `animations.json`
2. Define the values. Format: `"Frame Number": Time Interval`
Example:
```
{
    "1": 0,
    "2": 0.025,
    "10": 0.01,
    "15": 0.025
}
```
**Explanation:**
You do not need to state the length of each frame. The only time that absolutely needs to be defined is the first frame. If you did not set a time for the frame, Cluckabunga will use the time from the last frame.
The `Time Interval` is how long the frame stays on the screen for.
**Important:** The frame number must be a string (meaning in quotes) because of how json decoding works.

## Building
Just build like a normal Xcode project. Sign using your own team and bundle identifier. You can also build the IPA file with `ipabuild.sh`.

## Credits
- [Cluckabunga] Original From @leminlimez
(https://github.com/leminlimez/Cluckabun)
for the main project and a lot of code.
- [kfd] From @felix-pb
for the exploit 'puaf_landa' code.
(https://github.com/felix-pb/kfd)
- [Cardinal] From @leminlimez (https://github.com/leminlimez/Cardina)
for Card Changer.
- Misaka for offsets.

## Suggestions and support
Let me know if you have a issue or a suggestion just create at the issues in the top;)
__________________________________________
