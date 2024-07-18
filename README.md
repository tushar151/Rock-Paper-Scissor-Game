**Hand Gesture Rock-Paper-Scissors Game**

This is a Rock-Paper-Scissors game implemented using OpenCV and the CvZone library for hand gesture recognition. The game allows a player to compete against an AI that makes random moves. The game uses a webcam to detect the player's hand gestures and determine the player's move.

**Requirements**
Python 3.x
OpenCV
CvZone
HandTrackingModule (part of CvZone)
NumPy

**Installation**
Clone the repository:

Copy code
git clone https://github.com/yourusername/hand-gesture-rps-game.git
cd hand-gesture-rps-game

Install the required packages:

Copy code
pip install opencv-python cvzone numpy
**
Usage**
Run the game:

Copy code
python main.py

Press s to start the game.

The game will countdown from 3, during which you should make your move using hand gestures:

Fist (all fingers down) for Rock
Open hand (all fingers up) for Paper
Peace sign (index and middle fingers up) for Scissors


**Code Explanation**
The main game loop captures video from the webcam, detects hand gestures, and overlays the appropriate images to display the game state. The game logic determines the winner based on the player's and AI's moves and updates the score accordingly.

**Main Components**

Hand Detection: Using the CvZone HandDetector to detect and track hand gestures.

Game Logic: Randomly generates AI moves and compares them to the player's moves to determine the winner.

Display: Uses OpenCV to display the game interface, including the countdown, player and AI moves, and the score.
