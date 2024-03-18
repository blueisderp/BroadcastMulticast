# Broadcast/Multicast Project
By Le Duong

This project demonstrates simple network communication protocols between nodes in a simulated network environment using Docker. It simulates Broadcast and Multicast distribution protocols between the main master (server) node and the multiple receiving client nodes. Whenever the server node sends out a message using either protocol, each client should respond with the following: 

  - Distribution Protocol (Broadcast/Multicast)
  - Time (ms) 
  - Source IP
  - Destination IP 
  - Source Port 
  - Destination Port 
  - Communication Protocol (UDP/TCP)
  - Length of message (bytes)

It order to simulate the network environment, I used Docker to create containers to serve as my server and client nodes. Please see the Compiling Instructions for steps on how to recreate this demo. 
 

## Compiling Instructions
All these commands should be executed in your CLI
    *the following commands were run on Mac iOS but should remian the same for other OS*

    1.  Install and open the directory for this project
        ```bash
        cd BroadcastMulticast
        ```
    2. Build the docker images and run the containers using the docker-compose.yml
        ```bash
        docker-compose up --build
        ```
    3. After running the demo, terminate the previous containers using:
        ```bash
        docker-compose down
        ```
    Note: You may be prompted to login to your Docker account, if so then use the command: docker login