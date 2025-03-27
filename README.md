
Access the Website here : [Algo-Graphix](https://algo-graphix.netlify.app/)

// all buttons are disabled when a algorithms is running or while grid generation and all mousedown events are ignored.

// constructer is the first function that runs when the component is created.

// componentDidMount() -> ensures that the grid initialises onlt once when the component is added to the DOM.

// create a node object with some properties for every row ans col.

// handleMouseDown(row, col)
//    Moving the start node
//    Moving the end node
//    Adding or removing walls
//    Adding weighted nodes
//    Adding station nodes (extra feature)

//         1️⃣If the pathfinding algorithm is running or the grid is being generated, then ignore the mouse event.
//         2️⃣Extracts the node object at the clicked position from the this.state.grid[row][col].
//         3️⃣If the clicked node is the start node (isStart === true) and weights or stations are not being added, then:
              Set this.startNodeChange = true → This tells the program that the user wants to move the start node.
//         4️⃣If the clicked node is the end node (isFinish === true) and weights or stations are not being added, then:
              Set this.endNodeChange = true → This tells the program that the user wants to move the end node.
//         5️⃣If the clicked node is a station node (isStation === true) and the user is not adding weights or stations, then:
              Set this.stationNodeChange = true → This tells the program that the user wants to move a station node.
//         6️⃣If the clicked node is not: A start node An end node A station node A wall And weight addition mode is active (this.addingWeights === 1), then:
              Set this.addingWeights = 2 → This marks the node as a weighted node.  Calls this.changeState(...) to update the node's class ("node-weight") and set the weight.
//          7️⃣ Adding a Station Node
//          8️⃣ Adding or Removing a Wall
![image](https://github.com/user-attachments/assets/2662522c-be72-469b-b535-0bfec3e03f98)


