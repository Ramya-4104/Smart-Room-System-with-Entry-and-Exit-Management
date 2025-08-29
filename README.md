# Smart-Room-System-with-Entry-and-Exit-Management
Project Overview:
This project focuses on the design and implementation of a Smart Room System with entry and exit management, developed to combine automation, energy efficiency, and security in a single solution. The system uses two sensors to detect entry and exit events, which are processed to maintain a real-time occupancy count of the room. Based on this count, the system controls connected devices (AC and light) and manages door access for security.

The approach began by identifying the problem of manual monitoring and inefficient energy usage in traditional rooms. We then designed a circuit in Logisim, where the sensors act as inputs and trigger logic operations to update the occupancy count. The outputs of this logic determine whether the AC and light should be turned on or off, and whether the door should remain locked or unlocked. For example, an entry event increments the count, an exit decrements it, and when the maximum threshold is reached, the system automatically locks the door while keeping devices active for user comfort.

The logic of the solution is straightforward:

Input Stage: Entry and exit sensors provide real-time signals to the system.

Processing Stage: The microcontroller (simulated using Logisim) updates the occupancy count and classifies the room as empty, full, or available.

Output Stage:

If the room is empty → AC and light turn off, door unlocked.

If the room has occupants but is not full → AC and light turn on, door unlocked.

If the room is full → AC and light stay on, door locked for security.

Through these steps, the final output is a system that responds intelligently to occupancy changes, ensuring energy savings, user comfort, and safety. The project demonstrates how simple sensor inputs, combined with logical circuit design, can create a responsive and automated smart environment.
