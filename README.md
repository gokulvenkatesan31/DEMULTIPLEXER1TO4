# DEMULTIPLEXER1TO4
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/b6d81e6c-81ec-4f91-ae42-832a68f8facc)
# Truth Table
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/bb0a83c7-b4f3-463b-b422-f2ff65b1a0ee)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/dcd56444-97dd-454b-bddf-c7472c4af1de)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/03fbbbdf-8ae3-4653-8047-7d4cbf555ccb)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/f48cc07d-c76f-4d1c-8907-11e99711b751)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/a3075cf9-55ba-4478-b20c-c7128badef04)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/e07386db-69b3-4a5f-945f-b38929b801ea)
# Program
```
module demux_1_4( input [1:0] sel, input i, output reg y0,y1,y2,y3);

always @(*)
 begin case(sel)
 2'h0: {y0,y1,y2,y3} = {i,3'b0};
 2'h1: {y0,y1,y2,y3} = {1'b0,i,2'b0};
 2'h2: {y0,y1,y2,y3} = {2'b0,i,1'b0};
 2'h3: {y0,y1,y2,y3} = {3'b0,i};
 default: $display("Invalid sel input");
 endcase
 end
 endmodule
```
# Output
![319912662-9ff8f11d-da98-4881-bcdd-06c733fbaa6b](https://github.com/gokulvenkatesan31/DEMULTIPLEXER1TO4/assets/123715763/41276695-d19a-4058-bf16-7e7e38e48c77)
