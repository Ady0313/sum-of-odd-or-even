 sum-of-odd-or-even




#include<stdio.h>

void even()
{
//Variable Declaration
int r,sum=0;

// Taking Range
printf("Last Number To Sum up :\n");
scanf("%d",&r);

//Trying Loop
for(int g=0;g<r;++g)
    {
        if(g%2 ==0)
        {
        sum +=g;
        }
    }
    
    // Displaying Result
    printf("Result : %d",sum);
}


void odd()
{
//Variable Declaration
int r,sum=0;

//Taking Range
printf("Last Number To Sum up :\n");
scanf("%d",&r);


//Trying loop
for(int g=0;g<r;++g)
    {
        if(g%2 !=0)
        {
        sum +=g;
        }
    }
    //Displaying Resul
    printf("Result : %d",sum);
}



int main()
{

//Variable Declaration    
int opt;


//Taking Cases
printf("Sum Of (1 for Even ,2 for Odd) Upto a range :\n");
scanf("%d",&opt);


//Applying Case
switch(opt)
{
    case 1:
        even();
        break;
    case 2:
        odd();
        break;
    default:
        printf("Provide Correct Input");
        break;
}

return 0;    
}
