module allgates_tb;
reg A,B;
wire AND,OR,NOTA,NOTB,NAND,NOR,XOR,XNOR;
allgates dump(.A(A),.B(B),.AND(AND),.OR(OR),.NOTA(NOTA),.NOTB(NOTB),.NAND(NAND),.NOR(NOR),.XOR(XOR),.XNOR(XNOR));
initial begin
A=0;B=0;
#1A=0;B=1;
#1A=1;B=0;
#1A=1;B=1;
#1 $finish;
end
initial begin
$dumpfile("allgates.vcd");
$dumpvars(1,allgates_tb);
end
always@(*)
$display("INPUTVALUES: A=%b B=%b OUTPUTVALUES: AND=%b OR=%b NAND=%b NOR=%b XOR=%b XNOR=%b",A,B,AND,OR,NOTA,NOTB,NAND,NOR,XOR,XNOR);
endmodule
