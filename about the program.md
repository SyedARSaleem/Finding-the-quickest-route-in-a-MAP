# Finding-the-quickest-route-in-a-MAP

# Breadth First Search: 
The breadth first search was not that difficult to make. I made the use of queue data structure which 
allowed me to first access the paths pushed into the list first. I used a for loop to iterate through the non 
visited child of a node recursively in a while loop. Using a while loop, I ensured that all the possibilities 
have been checked before giving me the shortest path.  
I made a set of values passed in the queue which was the path currently being explored and the distance 
took to reach that path. In that way I could compare the distances of the valid paths and erase the paths 
larger than the rest. 
# Depth First Search: 
The code used in this search was similar to the Breadth First Search but, a stack data structure was used 
which meant the data pushed last will be used first, so we were able to explore the depth of a graph first 
recursively. 
# A* Search: 
A* search wasn’t as straight forward as the rest of the algorithms as it needed a heuristic value to start 
with. This could have been achieved easily by roughly calculating the distance of each node to the goal 
node, but this method could not be used as the goal state was based on the input of the user and 
therefore was unknown beforehand. 
So after a bit of thinking, I thought of giving vector coordinates to each city in the graph by manual 
calculation. I made a list of all the vector coordinates for and based on the goal state provided by the 
user, I calculated the distance between a required node and the goal state using Pythagoras theorem. 
For the working of the A* search, I used a priority queue which made sure that the data with the 
minimum calculated f(x) value was the first one to be used to find the goal node. I stored a set of values 
in the queue i.e. path, the actual distance of the path and the estimated distance of the path calculated 
using the heuristic values. 
When the goal state is reached the graph is terminated. This way the A* search doesn’t have to go 
through all the possible paths to find the shortest path.
