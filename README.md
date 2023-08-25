# Capture-The-Circle
Hand Tracking Game using MediaPipe, OpenCV and Python

Objective of this Game: Green Circles will appear on the Screen one at a time and we have to "Capture" then using the Red Circle on our Index Finger Tip.

Explanation:
1. CreateCaptureCircle()

   This function creates a circle randomly on the screen.

   Constraints:

         x Co-ordinate: 50 ≤ x ≤ 600

         y Co-ordinate: 50 ≤ y ≤ 400

      These constraints are Taken into Consideration in accordance with the Size of the Screen being Displayed (640 px, 480 px).

3. The while loop checks if the Video being captured using the Webcam is opened and takes the frames of the video as input.
   It then determines whether a Hand is in Frame or Not. If found, it assigns 21 Landmark Points and displays them along with a Red "Capturing Circle" on the Tip of the Index Finger.

   It calls the CreateCaptureCircle() function to create a random circle on the screen.
   Then it tracks the movement of the hand using Landmark Points and determines if the Capturing Circle (Red) has Touched the Circle to be Captured (Green) or Not.
   If the two Circle Touch, then the Captured Circle Disappears and Score is Increased by 1 point.

5. This goes on until the User Presses the "q" button.
