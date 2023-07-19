# ASIC_Design
Designing Complex ASIC  using system verilog

Problem-1: Designing Synchronous Bridge with Unequal data size.
        >> Input side: clk,rst,vld_i, [3:0] data_in
        >> Output Side: clk,rst, Vld_o, [4:0]data_out
      >>> The Interesting thing is The width of input is 4 bit and output is 5 bit
      >>> there is no handshake i.e No ready either at input or Output.
      
Solution: i have implemented using 2 approaches in system verilog.
        Solution-1:sync_bridge.sv >> Here , im going with most linient approach by taking a 20 bit buffer and 2 pointers wr 7 rd.
        Solution-2: Here, a more efficient and optimised solution is presented.
