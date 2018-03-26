# logical-equation
#include <stdio.h>

void bin(unsigned n)
{
    unsigned i;
    for (i = 1 << 2; i > 0; i = i / 2)
      (n & i)? printf("1"): printf("0");
}

int main(void)
{
    int var=1,i;
    printf("ABC   A+(B+C)\n");
    for(i=0;i<=7;i++)
    {
      bin(i);
      if(i==0)
      {
        var=0;
      }
      printf("\t%d",var); 
      printf("\n");
      var=1;
    }
}
