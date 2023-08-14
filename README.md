# Simulation-of-PRMA
### Simulation of PRMA and analysis

# Hybrid Access Schemes Packet Reservation Multiple Access (PRMA)

## BRIEF THEORY (Introduction) 

It is an implicit reservation scheme, where a fixed length TDMA Frame repeats periodically. Unlike the DAMA (explicit reservation), the controller does not play any role in reserving the TDMA slots for the contenting end-users. The controller (e.g., base station or satellite) announces the slot assignment prior to the commencement of TDMA frame. The end-users whose ID is announced may continue using their respective reserved slots. 

## ALGORITHM 

Reservation in PRMA 

In each frame, vacant slots can be found of by contenting end-users from the announcement by controller.  
Slots could be vacant due to an end of data transmission when the reserved slots are relinquished by the end-user and due to collisions in that slot in previous round. 
Contenting end-users may access an idle slot using Aloha. If a contenting end-user is successful in transmission, then the controller reserves the slot for that end user while others continue to contend in other idle slots. 
 
1)	Here list ‘r’ represents announcement by controller, list ‘l’ represents individual TDMA frames.
2)	Initially end-users are assigned randomly.
3)	Parameters considered in the simulation are no. of frames, no. of slots, slot duration which will remain constant throughout the frame. Bit rate of the sender and transmission data sizes are considered to be Uniform Distribution.
4)	From slot duration and source rate, size of the data that can be transmitted in that slot is calculated, remainder is forwarded to the next frame.
5)	 When a slot is idle, reservation is achieved through p-persistent Slotted Aloha. If a slot is successfully allocated, task size using the same distribution is allocated.

## Inference

Mean Source Rate and Mean Task Size exhibited linear relationship based on the input values and had a correlated behaviour with percentage of filled slots. 
Percentage of filled slots and number of collisions varied non-linearly with respect mean source rate and mean task size. With increase in mean task size and mean source rate, the reserved users transmitted data completely across less frames thereby increasing the collisions for reserving the empty slots. Hence, we observe for the input numerical values there is an increase in number of collisions and decrease in number of filled slots.  

