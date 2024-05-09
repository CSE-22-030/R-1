// SCIENTIFIC CALCULATOR : 82MS//
#include<stdio.h>
#include<math.h>
int main(){
    int a=1,b=1,choice,i,j,k,x=1,d=1,e=1,f=1;
    float r;
    printf("Enter the 1st number:");
    scanf("%d",&a);
    printf("Enter the 2nd number:");
    scanf("%d",&b);
    printf("PLEASE READ THE INSTRUCTIONS GIVEN BELOW\n");
    printf("Enter 1 to add.\n");
    printf("Enter 2 to subtract.\n");
    printf("Enter 3 to multiply.\n");
    printf("Enter 4 to divide.\n");
    printf("Enter 5 to perform modulus operation.\n");
    printf("Enter 6 to perform permutation & combination operations.\n");
    printf("Enter 7 to perform power operation.\n");
    printf("Enter 8 to perform sin.\n");
    printf("Enter 9 to perform cosine.\n");
    printf("Enter 10 to perform tangent.\n");
    printf("Enter 11 to perform logarithm addition.\n");
    printf("Enter 12 to perform logarithm subtraction.\n");
    printf("Enter 13 to perform logarithm multiplication.\n");
    printf("Enter 14 to perform logarithm division.\n");
    printf("Enter the choice:");
    scanf("%d",&choice);
    switch(choice){
        case 1:r=a+b;    //ADDITION
        printf("Result of addition=%f",r);
        break;
        case 2:r=a-b;     // SUBTRACTION
        printf("Result of subtraction=%f",r);
        break;
        case 3:r=a*b;	  // MULTIPLICATION
        printf("Result of multiplication=%f",r);
        break;
        case 4:r=a/b;      // DIVISION
        printf("Result of division=%f",r);
        break;
        case 5:r=a%b;    // MODULUS
        printf("Result of modulo operation=%f",r);
        break;
        case 6:    // COMBINATION AND PERMUTATION
        		   // TO PERFORM THIS OPERATION YOU NEED a>b 
        for(i=1;i<=a;i++){
            d=d*i;
        }
        x=a-b;
        for(j=1;j<=x;j++){
            e=e*j;
        }
        for(k=1;k<=b;k++){
            f=f*k;
        }
        r=(d)/(e*f);
        printf("Result of combination operation=%f\n",r);
        printf("Result of permutation operation=%f",(r*f));
        break;
        case 7:r=pow(a,b);
        printf("Result of power operation=%f",r);
       break;
       case 8:   // SIN FUNCTION
       r=sin(a+b);
       printf("Result(in sin)=%f",r);
       break;
       case 9:  // COSINE FUNCTION
       r=cos(a+b);
       printf("Result (in cos)=%f",r);
       break;
       case 10:   // TANMGENT FUNCTION
       r=tan(a+b);
       printf("Result(in tan)=%f",r);
       break;
       case 11:	//  LOGARITHM ADDITION
       r=log(a+b);
       printf("Result=%f",r);
       break;
       case 12:   //LOGARITHM SUBTRACTION
       r=log(a-b);
       printf("Result=%f",r);
       break;
       case 13:    //LOGARITHM  MULTIPLICATION
       r=log(a*b);
       printf("Result=%f",r);
       break;
       case 14:    // LOGARITHM DIVISION
       r=log(a/b);
       printf("Result=%f",r);
       break;
       default:printf("This calculator does not support this kind of operations.");
       break;
}
return 0;
}