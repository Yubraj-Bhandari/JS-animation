Initial Variables:

posX and posY start at 0, representing the initial top-left corner.
step is the number of pixels moved per frame (adjust this to control speed).
maxPos is set to 350, which is the farthest the element can move (the container is 400x400px, and the element is 50x50px, so 400 - 50 = 350).
Movement Logic:

Side 1 (Move Right): The element moves along the top edge (increasing posX).
Side 2 (Move Down): The element moves down along the right edge (increasing posY).
Side 3 (Move Left): The element moves left along the bottom edge (decreasing posX).
Side 4 (Move Up): The element moves up along the left edge (decreasing posY).
setInterval():

Every 10ms, the frame() function is called to update the position of the #inside element along one of the sides.
Once the element completes each side of the square, the side variable changes to indicate movement to the next side.
Stopping Condition:

Once the element reaches back to the top-left corner (when both posX and posY are 0 again), the clearInterval(id) stops the movement.
How It Works:
The element starts at the top-left corner (posX = 0, posY = 0).
It moves to the top-right corner (posX = 350, posY = 0).
Then it moves to the bottom-right corner (posX = 350, posY = 350).
Next, it moves to the bottom-left corner (posX = 0, posY = 350).
Finally, it moves back to the top-left corner (posX = 0, posY = 0) and stops. -->
