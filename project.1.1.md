not.hdl 

CHIP Not {
    
    IN in;
    OUT out;
    PARTS:
    Nand(a=in,b=in,out=out);
}
![image](https://github.com/user-attachments/assets/2a23b64d-bcf5-4a2e-89df-c261dc78f316)


or.hdl
CHIP Or {
    IN a, b;
    OUT out;

    PARTS:
    Not(in=a,out=nota);
    Not(in=b,out=notb);
    Nand(a=nota,b=notb,out=out);
}
![image](https://github.com/user-attachments/assets/3876da77-e9ef-4ba2-90ca-21529405155d)


