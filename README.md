# PyGame_Soccer_Agent-main
I have used the ‘pygame’ python library to simplify loading assets and rendering the players and the field. The implemented program starts at the empty screen,
The various controls for the program are as follows:-

Press X to: Relocate players randomly.
Press B to: Show/hide the bounding boxes of objects.
Press Esc to: Quit the program.
Once the program has starter press X to relocate players
randomly. Doing this automatically computes the top 4
shortest paths to score a goal and displays the path lengths
as well as coloured lines of the paths to follow.
#The environment is modelled as a data structure containing the following information,
![image](https://user-images.githubusercontent.com/73772907/221599148-0899b3df-8832-45c3-ad34-3e5c70387dc8.png)
To find the shortest path from the kicker to the centre of the goal, the program performs a Depth First
Search over all positions of the blue team players. Each position checks whether a pass can be sent
from the current position to any of the teammates that have not been explored during DFS. To check
is a pass is possible, the program performs 2 tasks, given a 2D point P 1 and P 2 ,
•
For each point P 0 as position of player that can receive a pass check if
o Minimum distance of the line from P 1 P 2 from P 0 > radius player
o Smallest rectangle containing P 1 and P 2 also contains P 0 .

![image](https://user-images.githubusercontent.com/73772907/221599402-9b9a551b-2468-427a-803f-e668a31724ca.png)

#sample
![image](https://user-images.githubusercontent.com/73772907/221599987-06594b3b-a98a-4635-93ed-9fe5cfc0ac90.png)

