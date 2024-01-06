# Overview

## How does Saint Mary's Gate work?

Saint Mary's Gate works using two main components: the server and the client. The server is responsible for handling all the game logic, and the client is responsible for displaying the game to the user.

All both are written in Java, and are open source. The Game Server is called Luna, and the Game Client is called Cassandra.

These two components uses a common library called <a href="https://github.com/st-mary/Coral">Coral</a> to communicate with each other. Coral is also written in Java, and is open source.

## Main Components

| Name                                 | Description                                                                                                                                                   |
|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <a href="Coral.md">Coral</a>         | Common library used across the St Mary Gate project, which provides essential functionalities and utilities that are shared between the game client & server. |
| <a href="Luna.md">Luna</a>           | Game server responsible for managing game logic, processing user inputs, and maintaining the overall state of the game world.                                 |
| <a href="Cassandra.md">Cassandra</a> | Game client responsible for handling user interactions and rendering the game interface.                                                                      |

<seealso>
    <category ref="related">
        <a href="Luna.md">Luna</a>
        <a href="Cassandra.md">Cassandra</a>
        <a href="Coral.md">Coral</a>
    </category>
</seealso>