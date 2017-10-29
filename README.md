# A-B-for-Input-Output-Practice-V-

A+B for Input-Output Practice (V)

Problem Description

Your task is to calculate the sum of some integers.

 
Input

Input contains an integer N in the first line, and then N lines follow. Each line starts with a integer M, and then M integers follow in the same line. 

 
Output

For each group of input integers you should output their sum in one line, and with one line of output for each line in input.  


Sample Input

2

4 1 2 3 4

5 1 2 3 4 5 


Sample Output

10

15 

解答：

#include<stdio.h>

main()

{

    int n,a,b,i,j,sum;
    
    sum=0;
    
    while(scanf("%d\n",&n)!=-1)
    
    {
    
        for(i=0;i<n;i++)
        
        {
        
            scanf("%d",&b);
            
            for(j=0;j<b;j++)
            
             {
             
                 scanf("%d",&a);
                 
                 sum+=a;
                 
             }
             
             printf("%d\n",sum);
             
             sum=0;
             
        }
        
    }
}
