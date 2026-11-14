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

