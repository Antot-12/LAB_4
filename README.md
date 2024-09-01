# 🏓 Pong Game with Networked Play

This repository contains a simple Pong game implemented in Python using the `turtle` module. The game supports two-player networked play over UDP sockets.

## 📋 Features

- 🕹️ **Single-player Mode**: Play the classic Pong game against yourself.
- 🌐 **Networked Multiplayer Mode**: Play Pong with a friend over a local network.
- 🖥️ **Server and Client Architecture**: One player acts as a server, and the other connects as a client.
- 🎨 **Graphical Interface**: Implemented using Python's `turtle` module, providing a simple yet fun interface.

## 🚀 Getting Started

### Prerequisites

- Python 3.x installed on your machine.
- Basic knowledge of running Python scripts.

### 🛠️ Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Antot-12/LAB_4.git
    cd LAB_4
    ```

2. **Run the server:**
    - Navigate to the directory and run the server script.
    ```bash
    python server.py
    ```
    - The server will start listening for incoming connections.

3. **Run the Pong game:**
    - There are two client scripts available:
        - `client1.py` (Client 1)
        - `client2.py` (Client 2)

    - Start the first client:
    ```bash
    python client1.py
    ```

    - Start the second client:
    ```bash
    python client2.py
    ```

4. **Play the game:**
    - The game window will appear, and you can start playing. Use the keyboard to control the paddles.

### 🎮 Controls

- **Client 1 (Left Paddle):**
  - `W` - Move paddle up.
  - `S` - Move paddle down.

- **Client 2 (Right Paddle):**
  - `Up Arrow` - Move paddle up.
  - `Down Arrow` - Move paddle down.

### ⚙️ How It Works

- **Server (`server.py`)**: 
  - The server script listens for incoming data packets from the clients. 
  - It maintains a list of clients and relays messages between them, enabling synchronized gameplay.

- **Client (`client1.py` and `client2.py`)**:
  - Each client script manages the game logic and interacts with the server to send and receive updates about the ball's position and the scores.
  - The game state is updated based on the data received from the server, ensuring that both clients see the same game state.

### 🛠️ Customization

You can customize the game settings such as ball speed, paddle size, and window size by modifying the constants defined at the beginning of the scripts.

### 🐞 Troubleshooting

- **Connection Issues**: Ensure that both the server and clients are on the same network and that the correct IP address and port are specified.
- **Lag or Delays**: Network performance can affect the gameplay experience. If you encounter issues, try playing on a faster network or reducing the game speed.

---

Enjoy the game! 🕹️
