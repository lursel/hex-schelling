# java-swing-hexes

This is a bare-bones implementation of hexagonial tiles in a 2D environment using JavaSwing.

I have included some basic function of generating, placing and moving agents on a topological map.

The implementation is based on Red Blob Games fantastic guide on hexagonal grids (https://www.redblobgames.com/grids/hexagons/) and how to implement them (https://www.redblobgames.com/grids/hexagons/implementation.html).

The relevant java file is /src/gui/Grid.java, which is the JPanel that draws the game world. This is the only class that needs to do mathy polygonial stuff. Agents and the gameworld classes use the usual 2d coordinate system just as they were using square tiles.

The rest of the files are simply to make this work as a demo so you can see how the world looks like. Inside /src/simulation/Simulation.java, you can adjust the number of hexes (by changing world size X and Y) and the number of agents and ticks (rounds). If you want to increase the size of a hexagon, adjust the HEXSIZE variable inside the Grid.java class.