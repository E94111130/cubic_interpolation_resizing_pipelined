# cubic_interpolation_resizing_pipelined
1.  using shift reg to implement pipelined circuit, temp<=img_addr_update; shift<=temp; therefore shift signal is 2 clock late compared to a_update.
2.  predicting shift logic without divider to minimize the area and the calculating time is made by a method called  "NOT to REDUCTION" then it's clear to see how this algorithm works.
3.  img_ROM is negedge sensitive.
4.  using horner's method to reduce the number of multiplier also to minimize the area, in this design i only use 4 multiplier and 3 of them for polynomial calculation the other one for the address calculating and there's no divider in this circuit, and i think it's the biggest improvement for me. 
