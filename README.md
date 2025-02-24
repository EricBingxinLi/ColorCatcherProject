
COLOR CATCHER
A Visual & Auditory Reaction Game

DESCRIPTION
Test your reflexes and cognitive speed in this color-word matching game! Words fall from the top of the screen with mismatched colors - quickly decide whether the word's meaning matches its display color before it reaches the bottom. Features dynamic difficulty scaling, sound effects, and retro-style animations.

KEY FEATURES

1.Falling/Rotating Text Challenge

2.Sound Effects (Success/Failure)

3.High Score Tracking System

4.Animated Intro Screen

5.Responsive Click Zones

6.Dynamic Speed Scaling (Faster as you score!)

SETUP INSTRUCTIONS

  Requirements

    Processing 4.0+

    Minim Audio Library (Install via Processing's Contribution Manager)

  File Structure

    ColorCatcher/  
    ├── data/  
    │   ├── FAILURE.wav  
    │   ├── SUCCESS.wav  
    │   └── thememusic.mp3  
    ├── ColorCatcher.pde  
    └── Kids Magazine.ttf (optional custom font) 
    
  Launch

    Open ColorCatcher.pde in Processing

    Click Run (▶️)

  HOW TO PLAY

    LEFT CLICK (0-450px): "MATCH" if word/color align

    RIGHT CLICK (450-900px): "DON'T MATCH" if they don't

    CIRCLE BUTTON (800,800): Change screens

GOAL: Survive as long as possible - text speeds up with higher scores!


CUSTOMIZATION OPTIONS

Modify Colors/Words
Edit the colors[] and words[] arrays:

color[] colors = {#FF0000, #00FF00, ...}; 
String[] words = {"RED", "GREEN", ...};

Adjust Difficulty

Change speed modifiers:
yPosition += 0.8 * score; // Current speed formula

Custom Sounds
Replace FAILURE.wav/SUCCESS.wav in /data (keep filenames)

TROUBLESHOOTING

No Sound Effects?

Confirm files are 16-bit WAV format

Check console for "Sound1 loaded: true" messages

Try Sound1.setGain(10); before play()

Game Logic Issues?
Add debug prints to check isMatching value:

println("Current Match Status:", isMatching);

DEPENDENCIES

Minim 2.2.2+ (Audio handling)

Processing Core Libraries

LICENSE
MIT License - Free for educational/modified use. Attribute if redistributed.

ACKNOWLEDGMENTS

Minim Audio Library by Damien Di Fede

Sample sounds from mixkit.co
