# CC1350_Networking_with_Dynamic_Source_Routing
Used C++ in conjunction with PICOS to implement a Dynamic Source Routing protocol across multiple CC1350 microcontrollers to allow each controller to wirelessly store and retrieve data from each controllers database that was on the network group.
## Description
The first thing a new controller would do is broadcast a packet indicating the desired group they want to join. The new controller will then receive a confirmation packet including their group id upon successfully joining the group. Once a controller is part of a group they can read/write entries in the databases of any other controller on the network by sending a packet indicating the id of the sender and receiver and a flag of whether they wish to read or write to the database. The packet then includes whatever additional information is required by the action, such as an element index in the case of a read request or a value to write in the case of a write request. 
Each controller is always receiving packets but only act on the messages received if the receiver id matches the controller's id.
## Important Skills
- Low level programming with minimal memory.
- Network communication with collision detection.
- Waveform and Signal processing.
- Low level database management and manipulation.
- Dividing Tasks between other two members to ensure efficient completion.

