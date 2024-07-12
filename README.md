## Algorithm for Bit Stuffing

1. Start
2. Initialize the array for transmitted stream with the special bit pattern `01111110` which indicates the beginning of the frame.
3. Get the bit stream to be transmitted into the array.
4. Check for five consecutive ones and if they occur, stuff a bit `0`.
5. Display the data transmitted as it appears on the data line after appending `01111110` at the end.
6. For de-stuffing, copy the transmitted data to another array after detecting the stuffed bits.
7. Display the received bit stream.
8. Stop



## Algorithm for Byte Stuffing

1. Start
2. Append `DLE STX` at the beginning of the string
3. Check the data for the `DLE` character; if `DLE` is present in the string (e.g., `JKODLE`), insert another `DLE` in the string (e.g., `JKODLEDLE`)
4. Transmit `DLE ETX` at the end of the string
5. Display the string
6. Stop
