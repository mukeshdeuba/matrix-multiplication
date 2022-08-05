# matrix-multiplication
this is c program for matrix multiplication


#include<stdio.h>
#include<conio.h>
#include<math.h>
int main()
{
    int i,j,k;
    int mat1[3][3];
    int mat2[3][3];
    int mat3[3][3];
    printf("enter the matrix elements matrix:\n");
    for(i=0;i<3;i++)
    {
         for(j=0;j<3;j++)
         {
           scanf("%d",&mat1[i][j]);
         }
        
    }
    printf("\n\n");
for(i=0;i<3;i++)
    {
         for(j=0;j<3;j++)
         {
           printf("%d\t",mat1[i][j]);
         }
        printf("\n");
    }
    printf("\n\n");
    printf("enter the matrix elements matrix:\n\n");
    for(i=0;i<3;i++)
    {
         for(j=0;j<3;j++)
         {
           scanf("%d",&mat2[i][j]);
         }
        
    }
    printf("\n\n");
for(i=0;i<3;i++)
    {
         for(j=0;j<3;j++)
         {
           printf("%d\t",mat2[i][j]);
         }
        printf("\n");
    }
    printf("the matrix after matrix  multiplicaion is:\n");
    for(i=0;i<3;i++)
    {
         for(j=0;j<3;j++)
         {
          int sum=0;
          for(k=0;k<3;k++)
          {
           sum=sum+mat1[i][k]*mat2[k][j];   
          }
          mat3[i][j]=sum;
           printf("%d\t",mat3[i][j]);
         }
        printf("\n");
    }
    getch();
    return 0;

}
