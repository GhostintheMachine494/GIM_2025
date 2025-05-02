# GIM_2025
This is the final repo containing all of the code for the 2024-2025 GIM team. The team was made up of Ben Wilson, Dawson Franklin, Dingding Ye, Hong-Ye Wang, Lindsey Russ, Natalia Mendiola, and Prahalad Chari. 

-------- Distributed Code Overview ------------

The dist_alg_test contains the code to run the most up-to-date version of the distributed algorithm. The code for one board is controller and the other is beta. When we ran it it would hang on reads and writes in the for loop of the algorithm. Easiest possible fix is to remove the pipelining pragmas within the for loop and see if that will then work. If that doesn't work, more detailed analysis will be necessary. 

The distributed_xor_cpp contains the algorithm HLS code without having been compiled. 

The fifo_test_source is the files for a successful proof of concept of the FIFO working.

The simple_packet_test contains the files for the successful test of sending packets across the board. Note, it is possible to hook up the pins within the same board and ensure you are receiving the data within a single board.

The split_model_logic folder contains the simulated XOR algorithm running across two boards. 

**Note: all of this was developed off a previous and flawed version of the XOR problem. Would recommend moving to the newest version of the XOR GIM implementation.
