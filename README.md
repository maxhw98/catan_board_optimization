# Catan Board Optimization using graphs in python
## Using a graph theory generalization of Catan board game to create the most balanced board setup

The outcome of this project was actually pretty surprising and I found a great board setup algorithm despite setting out to just practice my graph skills. I used a scipi package cause I have built graphs out by scratch in java for data structures and wasn't really feeling like doing it again. On to the algorithm tho, you can achieve an optimally balanced board equal to one with a desert in the middle (mathematically optimal but not really common as people seem to dislike it) with a desert on the outside if you follow a specific pattern.

### Setup algorithm:
Start with the desert in outer ring, but in the middle of an edge (i.e. not in a corner). Start with the A tile on the opposite corner and start going from there but when you skip the desert, go around rather than skip over the desert. This preserves all the correct adjacency of the numbers. If you look at the graphic I made in the article/jupyter notebook file it is more detailed and outlines proof for everything.  

Pretty interesting stuff and it was good to practice my graph theory stuff. If you're curious check out the .ipynb file on this repo, it'll render in HTML with no dependancies, and if you have jupyterlab and pandas you can play with it, set up a unique board of your own and see all the settlement locations and relative balance scores!