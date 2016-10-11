# JL
C++ Problems

1.给一堆vertex，他们本来是有序的排列成一列的，比如a->b->c->d, 但是这个序列 是不知道的，已知的是两两之间的先后关系，比如a->b, a->d, b->c, c->d， 然后让 回复这个序列

Ans: matrix

2.题目大意如下,请注意输入输出的格式,这里有309 digits 的要求:

The fuel control mechanisms have three operations:

1) Add one fuel pellet
2) Remove one fuel pellet
3) Divide the entire group of fuel pellets by 2 (due to the destructive energy released when a quantum antimatter pellet is cut in half, the safety controls will only allow this to happen if there is an even number of pellets)

Write a function called answer(n) which takes a positive integer as a string and returns the minimum number of operations needed to transform the number of pellets to 1. The fuel intake control panel can only display a number up to 309 digits long, so there won't ever be more pellets than you can express in that many digits.

For example:
answer(4) returns 2: 4 -> 2 -> 1
answer(15) returns 5: 15 -> 16 -> 8 -> 4 -> 2 -> 1

Test cases
==========

Inputs:
    (string) n = "4"
Output:
    (int) 2

Inputs:
    (string) n = "15"
Output:
    (int) 5
    
    
IDEA：
 1). Class BigInt  with subclass  {operations a. +1 b. -1 c./2}
 2). Algrithm %4 = 3 => +1
            %4 = 1 => -1
            
            
3.class Pixel{
    - unsigned char r, g, b; // r:red, g: green, b:blue; max = 256
    
    - "+": (a+b)/2           // 注意a+b 可能越界 
    
    - "-": |a-b|   
    
    - "=";
    
    - "<<" : output "pixelred = r, pixelgreen = b, pixelblue = b. "
    
    － construct -(r,g,b)
    
                - (0,0,0)    //defalt
                
                - (pixel)
                
    - function pixel blend - pixel blend(pixel a, piexl b,int n) //(n<=100)
    
                           - pixel blend(pixel b, int n) =blend(pixel a, piexl b,int n)
                           
}


4.Dynamic Programming
https://www.zhihu.com/question/23995189









