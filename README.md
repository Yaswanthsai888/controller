# controller
 code combines webcam input with hand and body pose estimation to control character movement in a game by recognizing specific hand gestures and simulating keyboard inputs accordingly.

 A Python script for controlling a character in a game using hand gestures captured through a webcam. Here's a brief description of what the code does:

It imports the necessary libraries, including OpenCV for webcam access, the MediaPipe library for hand and body pose estimation, and PyAutoGUI for simulating keyboard input.

The code sets up the webcam capture and initializes some variables to track hand and character positions.

It enters a loop where it continuously captures frames from the webcam.

Inside the loop, it processes the captured frame using MediaPipe's Holistic and Hands models to detect hand and body landmarks.

It calculates the positions of the left and right shoulders and the midpoint between them, which is used to control character movement in the game.

The code simulates keyboard input based on hand gestures. For example, it presses the 'left' or 'right' keys when it detects the corresponding hand movements. It also simulates 'up' and 'down' key presses based on hand positions.

Additionally, it checks for a specific gesture where both hands have two fingers extended, and if detected, it simulates a 'space' key press, possibly for character jumping in the game.

It displays the processed frame with visual cues, such as a center arrow and circles, to indicate the character's position and reference points.

The loop continues to process frames until you manually close the window.
