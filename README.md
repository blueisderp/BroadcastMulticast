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


## Compiling and Testing Instructions
    
1. Ensure the following files are located in the same file directory: 
    
            - client.py
            - master.py
            - Dockerfile_client
            - Dockerfile_master
            - docker-compose.yml

(Note: Files must be named exactly as seen above.)

2. Make sure the current working directory of the terminal is set to where all the files are located.

            cd [folder_name]

3. Login to Docker using the command:

            sudo docker login 

4. Build the Docker images and run the containers by running the command:

            sudo docker-compose up --build

5. Terminate and remove the containers and network with the command: 

            sudo docker-compose down