# Smart Traffic Management System Simulator

### Overview
The **Smart Traffic Management System Simulator** is a project designed to emulate real-world urban traffic management. It aims to optimize traffic flow in a city using data structures. This project was assigned to us for our data structures course. 


---

### Features

#### **City Traffic Network**
- Represents the city's road network as a weighted, directed graph.
  - **Nodes:** Intersections.
  - **Edges:** Roads between intersections with weights based on travel times or congestion levels.
- Dynamic addition and removal of roads and intersections.
- Visualization of the network structure.

#### **Vehicle Routing System**
- Calculates optimal routes for vehicles using **Dijkstra's Algorithm**.
- Dynamically updates routes based on changing traffic conditions.
- Tracks vehicle movements across the network.

#### **Traffic Signal Management**
- Dynamically adjusts traffic signal durations based on vehicle density.
- Manages intersections using a **priority queue** to reduce congestion.
- Supports an emergency override for critical situations.

#### **Congestion Monitoring**
- Monitors real-time vehicle counts on each road segment using a **hash table**.
- Identifies congestion zones and reroutes traffic using **BFS/DFS algorithms**.

#### **Emergency Vehicle Handling**
- Clears paths for emergency vehicles using **A* Search Algorithm**.
- Restores normal traffic flow after emergencies.

#### **Accident and Road Closure Simulation**
- Simulates road closures or accidents dynamically.
- Updates affected vehicle routes and recalculates traffic flow.

#### **Simulation Dashboard**
- Displays:
  - Traffic network graph.
  - Vehicle routes and positions.
  - Traffic signal statuses.
  - Congestion levels.
- Generates logs for all system actions, including rerouting and signal adjustments.

---

### Data Structures and Algorithms

#### **Data Structures**
- **Graph (Adjacency List):** Represents the road network.
- **Priority Queue:** Manages road order for signal adjustments.
- **Hash Table:** Tracks real-time vehicle counts.
- **Min-Heap:** Identifies the most congested roads.

#### **Algorithms**
- **Dijkstra's Algorithm:** Finds the shortest paths.
- **A* Search Algorithm:** Handles emergency vehicle routing.
- **BFS/DFS:** Detects congested or inaccessible zones.

---

### How to Run the Program

1. **Input Files:**
   - **road_network.csv:** Defines the road network (nodes and edges).
   - **vehicles.csv:** Lists vehicles (ID, start, and end points).
   - **traffic_signal_timings.csv:** Specifies initial signal durations.
   - **emergency_vehicles.csv:** Lists emergency vehicles (ID, start, end, priority).
   - **road_closures.csv:** Simulates road closures or accidents.

2. **Compilation:**
   - Use a C++ compiler (e.g., `g++`) to compile the program:
     ```bash
     g++ -o traffic_simulator traffic_simulator.cpp
     ```

3. **Execution:**
   - Run the compiled program:
     ```bash
     ./traffic_simulator
     ```

4. **Interactive Menu:**
   - Choose from the options provided to simulate various traffic scenarios.

---

### Sample Outputs
![Screenshot 2024-12-08 225958](https://github.com/user-attachments/assets/75b974b1-f456-4232-8c1e-099fd364254f)
![Screenshot 2024-12-08 230026](https://github.com/user-attachments/assets/4d844b67-f6df-4909-b44f-e4d63ffcd64c)
![Screenshot 2024-12-08 230101](https://github.com/user-attachments/assets/b29ca22d-bfc2-4267-8e1b-d1408ed6f434)
![Screenshot 2024-12-08 230127](https://github.com/user-attachments/assets/3a9a0a78-0a49-4395-bfdd-0836aab61a19)
![Screenshot 2024-12-08 230152](https://github.com/user-attachments/assets/0b212f62-8e21-4183-bc99-c07e8bec729d)
![Screenshot 2024-12-08 230235](https://github.com/user-attachments/assets/1dc8a212-c08d-48cb-b000-ea6bc9790bda)


