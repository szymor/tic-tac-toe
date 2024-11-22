# Tic-tac-toe

The game is implementation of an idea where two game clients connect to a server unaware of game logic, in this case Tic-tac-toe. Why is this limitation important? It may be beneficial to implement the logic in clients, as then it is possible to use existing infrastructure for communication. FTP servers with anonymous read and write access could be used for storage, whereas MQTT servers with unauthenticated access could be used to pass traffic in "real time", mildly speaking, as it was done in this proof of concept.

## Advantages

- low cost solution
- no requirements for specific server infrastructure
- possibility to use existing infrastructure

## Disadvantages

- low quality of service
- high latency (even a few seconds)
- acceptable only for turn-based games
