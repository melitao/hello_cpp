Task 2 Linker error msg: 

melitao@melitao-virtual-machine:~/hello_cpp$ g++ main.o -o tracker
/usr/bin/ld: main.o: in function `main':
main.cpp:(.text+0x3d): undefined reference to `distance(double, double, double, double)'
collect2: error: ld returned 1 exit status


Task 2 Compiler error:

melitao@melitao-virtual-machine:~/hello_cpp$ g++ -c main.cpp -o main.o
main.cpp: In function ‘int main()’:
main.cpp:7:75: error: expected ‘;’ before ‘return’
    7 |         std::cout << "Distance to target: " << d << " pixels" << std::endl
      |                                                                           ^
      |                                                                           ;
    8 |         return 0;
      |         ~~~~~~                                                             



Task 3 Question 4: Roughly how many lines of assembly were there with -O0 vs. -O2? Why would we want -O2 on the robot?

With -O0, there were about 8 lines of assembly, while -O2 only had about 3 lines. We want -O2 on the robot because it removes unnecessary instructions which helps the robot process information and respond to commands more quickly.
