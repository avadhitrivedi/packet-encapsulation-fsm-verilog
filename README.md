The following state machine takes incoming data (payload) and provide an output packet with payload data encapsulated between a 32 Bit header and footer. 
The header format includes a 16 bit payload length and 16 bit Sequence Number (count each incoming packet and assign the sequence number) while the footer is static (All 1’s). 
A packet of data is considered valid when data is provided with a valid as high, last signal indicates end of packet (High for one clock cycle).
Input ports of the module: clock, resetn, dataIn, validIn, lastIn.
Output ports of the module: dataOut, validOut, lastOut.
Note: Maximum Packet Length is 381 Words.
