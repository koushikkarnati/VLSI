# VLSI
Basic RTL Codes
module full_adder_dataflow(
    input  a,
    input  b,
    input  cin,
    output sum,
    output cout
);

assign sum  = a ^ b ^ cin;                // XOR for sum
assign cout = (a & b) | (b & cin) | (a & cin);   // Carry-out

endmodule
